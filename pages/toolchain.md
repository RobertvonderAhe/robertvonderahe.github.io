# Toolchain

Hier will ich einmal meine Erfahrungen im Arbeiten mit unterschiedlichen Tools zusammenfassen. Damit hoffe ich beschreiben zu können, was hier in meiner Erfahrung Best Practices Sind.

Diese Vorstellung erhebt an keiner Stelle Ansprüche von Objektivität oder Vollständigkeit.

---

## Was gibt es für Toolgruppen?

*Meine Persönliche Einteilung in Toolgruppen*

*Die Bezeichnbungen habe ich mir im Zweifel ausgedacht*

- Speichertools
- Prozesstools
- Entwicklungstools

---

### Speichertools

- Lokale Festplatten
- Mobile Datenträger (e.g. USB-Stick)
- Netzspeicher
- Cloudspeicher (e.g. Dropbox)
- SVN
- git
- Sharepoint (?)

---

#### Vergleich
| Typ | Vorteile | Nachteile |
|---|---|---|
| Lokal | Out-Of-The-Box <br> Alles Lokal und Offline Verfügbar | Keine Sicherung <br> Kein Backup |
| Mobil | OOTB <br> Einfacher Personenwechsel <br> Alles Lokal und Offline Verfügbar | Keine Sicherung <br> Kein Backup |
| Netz | Alle können bearbeiten <br> 

---
#### Fazit

Wenn möglich macht git für alle Sinn. Wenn der Mangel an Intuitiven GUIs eine zu große Hürde ist, sollte nach Usecase abgewogen werden zwischen SVN oder Cloudspeichern. 

---

### Prozesstools

- Projektmanagement (GANTT)
- Anforderungen
- Ticket-System
- Review-Tool
- Buildtool (nicht nur für Software)
- Testmanagement (Okay, das ist vermutlich nur im Engineering interessant)
- Wiki

---
#### Projektmanagement Tool

- Ressourcenplanung

Standalone:
Microsoft Project

---
#### Anforderungen

- Für konkrete Projekte
- Zum Arbeiten nach einer Art V-Modell 
- Traceability

---
#### Ticket System
Arbeitspackete (Tickets) Beschreiben
- Was soll gemacht werden
- Wer soll es machen
- Was ist schon passiert
- Was sind Probleme / muss noch geklärt werden
- Tickets Status zuordnen
- Tickets (verbleibenden) Stunden zuordnen

Standalone Beispiele:
- Whiteboard, Magnete, Zettel
- Trello

---
#### Verschiedene Tools von verschiedenen Bezugspunkten

| Ökosystem | github/gitlab | Atlassian | JetBrains | IBM | Polarion | Redmine | Windows |
|---|---|---|---|---|---|---|---|
| Projekt | - | - | YouTrack | - | Polarion | Redmine | 
| Anforderung | - | *PlugIn* | - | Doors | Polarion | - |
| Ticket | github/gitlab | JIRA | - | CRM | Polarion | Redmine | Azure |
| Review | github/gitlab | Bitbucket | Upsource | - | Polarion | - | Azure |
| Build | github/gitlab | Bamboo | TeamCity | - | - | - | Azure |
| Test | - | - | Qodana | - | - | - | Azure |
| Wiki | github/gitlab | Confluence | - | - | Polarion | Redmine | Azure |