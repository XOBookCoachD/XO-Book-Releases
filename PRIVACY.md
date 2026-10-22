# Datenschutzerklärung für XO/Book

**Verbindliche Fassung:** Diese deutsche Fassung ist die rechtlich verbindliche. Die englische Fassung weiter unten dient nur dem besseren Verständnis (*The German version is the binding one; the English version below is a convenience translation.*)

Stand: 22.10.2026

## 1. Verantwortlicher

Verantwortlich für die Datenverarbeitung im Sinne der Datenschutz-Grundverordnung (DSGVO) ist:

Dustin Struß  
Kurfürstenstraße 51  
45479 Mülheim an der Ruhr
E-Mail: dustin.struss@langenfeld-longhorns.de

Ein Datenschutzbeauftragter ist nicht benannt, da hierzu nach derzeitiger Einschätzung keine Verpflichtung besteht.

## 2. Überblick

XO/Book ist eine Desktop-Anwendung für Windows und macOS zum Erstellen von Football-Playbooks und zur Organisation von Coaching-Staffs. Die App ist grundsätzlich ohne Benutzerkonto und ohne Internetverbindung nutzbar. Personenbezogene Daten werden nur in den unten beschriebenen Fällen verarbeitet:

| Funktion | Daten verlassen Ihren Rechner? | Empfänger |
|---|---|---|
| Lokale Nutzung (Playbooks, Team-Dateien) | Nein | – |
| Absturzprotokoll | Nein (nur lokal) | – |
| Feedback senden (optional) | Ja, nur wenn Sie es absenden | GitHub |
| Automatische Updates | Ja | GitHub |
| Online-Zusammenarbeit (optional) | Ja | Supabase |

## 3. Lokale Nutzung ohne Konto

Playbooks (Dateiendung `.xobook`) und Team-Dateien (`.xoteam`) werden ausschließlich auf Ihrem Computer gespeichert. Es findet keine Analyse Ihres Nutzungsverhaltens (Analytics), kein Tracking, keine Werbung und keine Telemetrie statt. Der Entwickler erhält diese Dateien nicht.

## 4. Fehlerprotokolle und Feedback

**Lokales Absturzprotokoll.** Bei einem Absturz schreibt die App eine Protokolldatei in den lokalen Anwendungsdatenordner Ihres Benutzerkontos. Diese Datei wird **nie automatisch** übertragen. Sie können sie jederzeit selbst einsehen und löschen.

**Feedback senden.** Über *Help > Send Feedback* öffnet die App in Ihrem Browser ein vorausgefülltes Formular für ein GitHub-Issue. Vorausgefüllt sind die App-Version und der Name Ihres Betriebssystems. Ob und was Sie tatsächlich absenden, entscheiden allein Sie. Bitte beachten Sie, dass GitHub-Issues für andere Personen öffentlich sichtbar sein können; geben Sie dort keine personenbezogenen oder vertraulichen Daten an. Mit dem Absenden gelten die Datenschutzbestimmungen von GitHub (GitHub Inc., Microsoft, USA). Rechtsgrundlage für das Öffnen des Formulars ist Ihre Anfrage; die Verarbeitung nach dem Absenden erfolgt auf Ihre Veranlassung und unter der Verantwortung von GitHub.

## 5. Automatische Updates

Die App prüft bei GitHub (github.com, GitHub Inc., eine Tochter von Microsoft, USA), ob eine neue Version vorliegt, und lädt Updates von dort herunter. Dabei erhält GitHub technisch bedingt Ihre IP-Adresse und die üblichen technischen Anfragedaten (z. B. Zeitpunkt, angefragte Adresse, Browser-/Client-Kennung).

Rechtsgrundlage ist Art. 6 Abs. 1 lit. f DSGVO. Unser berechtigtes Interesse besteht darin, die Software sicher und aktuell zu halten. Soweit eine Übermittlung in die USA stattfindet, richtet sich diese nach den von GitHub bereitgestellten Garantien; Näheres finden Sie in den Datenschutzhinweisen von GitHub.

## 6. Optionale Online-Zusammenarbeit („Share with Coaches“ / „Join Team“)

Diese Funktionen sind freiwillig. Ohne sie werden keine Daten an den Online-Dienst übertragen.

### 6.1 Dienstleister

Für die Online-Funktionen nutzen wir Supabase (Supabase Inc., USA). Die Datenbank wird in der Region Frankfurt (eu-central-1) betrieben. Mit Supabase besteht ein Vertrag zur Auftragsverarbeitung (Art. 28 DSGVO). Soweit dabei Daten in die USA übermittelt werden oder von dort zugänglich sind, erfolgt dies auf Grundlage des EU-US Data Privacy Framework (sofern Supabase zertifiziert ist) und/oder der EU-Standardvertragsklauseln.

### 6.2 Welche Daten werden verarbeitet?

- **Konto:** E-Mail-Adresse, Passwort (bei Supabase Auth nur als Hash gespeichert, nicht im Klartext), Anzeigename.
- **Team:** Teamname, Team-Codes (zum Beitreten), Mitgliedschaft und Rolle (Coach oder Spieler).
- **Geteilte Team-Datei (Coaching Organization):** der Inhalt, den Coaches eingeben, z. B. Depth Charts mit Spielernamen, Zuständigkeiten im Staff, Self-Scout-Spieldaten, Trainingspläne und -skripte.
- **Änderungsprotokoll:** die letzten 100 Änderungen je Team, damit Mitcoaches nicht jedes Mal die ganze Datei laden müssen.
- **Präsenz („Presence“):** wer gerade online ist, und der Zeitpunkt der letzten Aktivität („last seen“). Solange das Coaching-Fenster geöffnet ist, wird dieser Zeitstempel alle paar Sekunden aktualisiert.
- **Anmeldung auf Ihrem Computer:** Ihre Anmeldung wird als sogenanntes Refresh-Token in den lokalen Einstellungen der App gespeichert, damit Sie nicht jedes Mal neu anmelden müssen. Beim Abmelden bzw. Löschen des Kontos wird es entfernt.
- **Vorbereitete Spielerfunktionen:** Die Datenbank enthält bereits Tabellen für Funktionen, die Playbooks für Spieler bereitstellen. Sofern Ihr Team diese Funktionen nutzt, können zusätzlich verarbeitet werden: an Spieler freigegebene Playbooks (einschließlich Seitenbildern), die auf einer Seite verbrachte Zeit sowie Quizantworten.

### 6.3 Rechtsgrundlagen und Rollenverteilung

- **Kontoinhaber (Coaches und Spieler):** Für die Daten, die zur Bereitstellung des Kontos und der Online-Funktionen nötig sind, ist die Rechtsgrundlage Art. 6 Abs. 1 lit. b DSGVO (Nutzung des Dienstes bzw. Vertrag).
- **Von Coaches eingegebene Daten über Spieler und andere Personen:** Hier ist das **Team (der Verein bzw. die Mannschaft)** der Verantwortliche. XO/Book stellt die Infrastruktur bereit und handelt insoweit als **Auftragsverarbeiter** nach Art. 28 DSGVO. Das Team entscheidet, welche Daten es eingibt, und braucht dafür eine eigene Rechtsgrundlage (z. B. Einwilligung oder berechtigtes Interesse) sowie ggf. eine Information der betroffenen Personen. Die erforderliche Vereinbarung zur Auftragsverarbeitung zwischen Team und Betreiber ist auf Anfrage unter dustin.struss@langenfeld-longhorns.de erhältlich.
- **Besondere Hinweise:** Bitte geben Sie **keine Gesundheitsdaten** (z. B. Verletzungen) und keine Daten von **Kindern** ein, wenn Ihr Team dafür keine tragfähige Rechtsgrundlage hat. Bei Jugendmannschaften kann die Einwilligung der Erziehungsberechtigten erforderlich sein.

### 6.4 Speicherdauer und Löschung

Die Daten werden gespeichert, bis das Konto bzw. das Team gelöscht wird. Sie können Ihr Konto jederzeit in der App löschen (*Help > Delete Online Account…* oder im Team-Menü, „Delete Account“). Das Konto wird sofort gelöscht. Geteilte Team-Dateien, bei denen Sie der einzige Coach sind, werden online gelöscht; gibt es weitere Coaches, bleiben sie für diese erhalten. Lokale Dateien auf Ihrem Computer bleiben unberührt. Sicherungskopien (Backups) bei Supabase können noch für einen begrenzten Zeitraum fortbestehen (höchstens 30 Tage).

## 7. Ihre Rechte

Sie haben nach der DSGVO folgende Rechte:

- Auskunft (Art. 15)
- Berichtigung (Art. 16)
- Löschung (Art. 17)
- Einschränkung der Verarbeitung (Art. 18)
- Datenübertragbarkeit (Art. 20)
- Widerspruch gegen Verarbeitungen auf Grundlage von Art. 6 Abs. 1 lit. f (Art. 21)
- Widerruf einer erteilten Einwilligung mit Wirkung für die Zukunft (Art. 7 Abs. 3)

Zur Ausübung wenden Sie sich bitte an dustin.struss@langenfeld-longhorns.de. Betreffen Ihre Daten Eingaben eines Teams (Abschnitt 6.3), wenden Sie sich bitte zunächst an den Verantwortlichen Ihres Teams; wir unterstützen diesen als Auftragsverarbeiter.

Sie haben außerdem das Recht, sich bei einer Datenschutz-Aufsichtsbehörde zu beschweren, z. B. bei der Behörde des Bundeslandes des Verantwortlichen: die Landesbeauftragte für Datenschutz und Informationsfreiheit Nordrhein-Westfalen (LDI NRW), Kavalleriestraße 2–4, 40213 Düsseldorf.

## 8. Pflicht zur Bereitstellung, automatisierte Entscheidungen

Sie sind nicht verpflichtet, personenbezogene Daten bereitzustellen. Sie sind nur für die Online-Funktionen erforderlich; ohne sie können diese nicht genutzt werden. Eine automatisierte Entscheidungsfindung einschließlich Profiling findet nicht statt.

## 9. Sicherheit

Die Übertragung zu den Online-Diensten erfolgt verschlüsselt (TLS). Zugriffsregeln in der Datenbank stellen sicher, dass jedes Team nur seine eigenen Daten lesen kann. Kein System ist jedoch vollständig sicher; wählen Sie ein starkes, einmaliges Passwort.

## 10. Änderungen

Wir passen diese Erklärung an, wenn sich die App oder die Rechtslage ändert. Es gilt die jeweils aktuelle Fassung.

---

# Privacy Policy for XO/Book (English version)

**Binding version:** The German version above is the legally binding one. This English version is provided for convenience only.

Last updated: 22 October 2026

## 1. Controller

The controller within the meaning of the General Data Protection Regulation (GDPR) is:

Dustin Struß  
Kurfürstenstraße 51  
45479 Mülheim an der Ruhr
Email: dustin.struss@langenfeld-longhorns.de

No data protection officer has been appointed, as there is currently assumed to be no obligation to do so.

## 2. Overview

XO/Book is a desktop application for Windows and macOS for creating football playbooks and organizing coaching staffs. The app can be used without an account and without an internet connection. Personal data is processed only in the cases described below:

| Feature | Does data leave your computer? | Recipient |
|---|---|---|
| Local use (playbooks, team files) | No | – |
| Crash log | No (local only) | – |
| Send feedback (optional) | Yes, only if you submit it | GitHub |
| Automatic updates | Yes | GitHub |
| Online collaboration (optional) | Yes | Supabase |

## 3. Local use without an account

Playbooks (file extension `.xobook`) and team files (`.xoteam`) are stored only on your computer. There is no analytics, no tracking, no advertising and no telemetry. The developer does not receive these files.

## 4. Error logs and feedback

**Local crash log.** If the app crashes, it writes a log file to the local application data folder of your user account. This file is **never sent automatically**. You can inspect and delete it at any time.

**Send feedback.** *Help > Send Feedback* opens a pre-filled GitHub issue form in your browser. The app version and the name of your operating system are pre-filled. You alone decide whether and what to submit. Please note that GitHub issues may be visible to others; do not include personal or confidential data. Once you submit, GitHub's privacy policy applies (GitHub Inc., Microsoft, USA). The legal basis for opening the form is your request; processing after submission happens at your initiative and under GitHub's responsibility.

## 5. Automatic updates

The app checks GitHub (github.com, GitHub Inc., a Microsoft subsidiary, USA) for new versions and downloads updates from there. For technical reasons, GitHub receives your IP address and the usual technical request data (e.g. time, requested address, client identifier).

The legal basis is Art. 6(1)(f) GDPR. Our legitimate interest is keeping the software secure and up to date. Where data is transferred to the USA, this is subject to the safeguards provided by GitHub; see GitHub's privacy information for details.

## 6. Optional online collaboration ("Share with Coaches" / "Join Team")

These features are voluntary. Without them, no data is sent to the online service.

### 6.1 Service provider

For the online features we use Supabase (Supabase Inc., USA). The database is hosted in Frankfurt (eu-central-1). A data processing agreement (Art. 28 GDPR) is in place with Supabase. To the extent data is transferred to, or accessible from, the USA, this is done on the basis of the EU-US Data Privacy Framework (where Supabase is certified) and/or the EU Standard Contractual Clauses.

### 6.2 What data is processed?

- **Account:** email address, password (stored by Supabase Auth only as a hash, not in plain text), display name.
- **Team:** team name, team codes (for joining), membership and role (coach or player).
- **Shared team file (Coaching Organization):** whatever coaches enter, e.g. depth charts with player names, staff responsibilities, self-scout game data, practice schedules and scripts.
- **Change log:** the last 100 edits per team, so that fellow coaches do not have to load the whole file every time.
- **Presence:** who is currently online, and a "last seen" timestamp. While the coaching window is open, this timestamp is refreshed every few seconds.
- **Login on your computer:** your login is kept as a refresh token in the app's local settings so you do not have to sign in every time. It is removed when you sign out or delete your account.
- **Prepared player features:** the database already contains tables for features that provide playbooks to players. If your team uses these features, the following may additionally be processed: playbooks shared with players (including page images), time spent per page, and quiz answers.

### 6.3 Legal bases and roles

- **Account holders (coaches and players):** for the data needed to provide the account and the online features, the legal basis is Art. 6(1)(b) GDPR (use of the service / contract).
- **Data about players and other persons entered by coaches:** here the **team (the club or squad)** is the controller. XO/Book provides the infrastructure and acts as **processor** under Art. 28 GDPR. The team decides which data it enters and needs its own legal basis (e.g. consent or legitimate interest) and, where applicable, must inform the persons concerned. The required data processing agreement between team and operator is available on request at dustin.struss@langenfeld-longhorns.de.
- **Special notes:** please do **not** enter **health data** (e.g. injuries) or data of **children** unless your team has a sound legal basis. For youth teams, consent of parents or guardians may be required.

### 6.4 Retention and deletion

Data is kept until the account or team is deleted. You can delete your account at any time in the app (*Help > Delete Online Account…* or the Team menu, "Delete Account"). The account is deleted immediately. Shared team files where you are the only coach are deleted online; if other coaches exist, the files remain for them. Local files on your computer are not affected. Backups at Supabase may persist for a limited period (at most 30 days).

## 7. Your rights

Under the GDPR you have the right to:

- access (Art. 15)
- rectification (Art. 16)
- erasure (Art. 17)
- restriction of processing (Art. 18)
- data portability (Art. 20)
- object to processing based on Art. 6(1)(f) (Art. 21)
- withdraw consent given, with effect for the future (Art. 7(3))

To exercise them, contact dustin.struss@langenfeld-longhorns.de. If your data was entered by a team (section 6.3), please contact your team's controller first; we support them as processor.

You also have the right to lodge a complaint with a data protection supervisory authority, e.g. the authority of the controller's federal state: the State Commissioner for Data Protection and Freedom of Information of North Rhine-Westphalia (LDI NRW), Kavalleriestraße 2–4, 40213 Düsseldorf, Germany.

## 8. Obligation to provide data, automated decisions

You are not obliged to provide personal data. It is only required for the online features; without it they cannot be used. There is no automated decision-making, including profiling.

## 9. Security

Transmission to the online services is encrypted (TLS). Access rules in the database ensure that each team can only read its own data. No system is completely secure, however; please choose a strong, unique password.

## 10. Changes

We update this policy when the app or the legal situation changes. The current version applies.
