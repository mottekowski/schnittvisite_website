# Abnahme vor Veröffentlichung

Stand: 11.10.2026. Noch offene Prüfungen; keine Veröffentlichung freigegeben.

## 1. Prüfung auf echten Handys

Die lokale Vorschau unter `127.0.0.1:8000` ist nur auf dem Entwicklungsrechner erreichbar. Auf einem Handy zeigt diese Adresse nicht die Vorschau dieses Rechners. Für echte Gerätetests wird zunächst eine ausdrücklich freigegebene, separate Testbereitstellung benötigt. Keine Netzwerkfreigabe oder Firewalländerung automatisch vornehmen.

Auf mindestens einem iPhone mit Safari und einem Android-Gerät mit Chrome prüfen und Gerät, Browser sowie Ergebnis dokumentieren:

| Prüfung | Erwartetes Ergebnis | Ergebnis |
| --- | --- | --- |
| Startseite im Hoch- und Querformat | Kein seitliches Überlaufen; Text und Foto passen | Offen |
| Größere Schrift beziehungsweise Browserzoom | Inhalte bleiben lesbar und bedienbar | Offen |
| Navigation zu Leistungen, Über mich, Preisen | Passender Abschnitt wird erreicht | Offen |
| Alle vier Preislisten durch Antippen | Jede Liste öffnet und schließt; Preise lesbar | Offen |
| Telefonnummer antippen | Telefon-App zeigt +49 174 3447677; keinen Testanruf auslösen | Offen |
| E-Mail-Link antippen | E-Mail-App öffnet passenden Empfänger; keine Nachricht senden | Offen |
| Impressum, Datenschutz und Cookie-Hinweise | Alle Seiten erreichbar; Rückkehr zur Startseite funktioniert | Offen |

## 2. Weitere Barrierefreiheitsprüfung

- Screenreader: Landmarks, Überschriften, Sprunglink, Bildbeschreibung, Preislistenstatus und Tabellenzuordnung prüfen. Kein Nachweis durch alleinige Prüfung des HTML-Codes.
- Auf allen rechtlichen Seiten die Tastaturreihenfolge und sichtbaren Fokus prüfen. Auf der Startseite sind Tab-Reihenfolge, Sprunglink und Preislisten bereits lokal geprüft.
- Weitere Browser sowie Zoom prüfen; keine vollständige Barrierefreiheit allein aus dem bisherigen Prüfbericht ableiten.

## 3. Inhaltsfreigabe und verbleibende Angaben

- [x] Kontaktangaben, Einsatzgebiet, Qualifikation seit 2009 und Fotoverwendungsrechte vom Nutzer bestätigt.
- [x] Herren-, Kinder- und Zusatzpreise vom Nutzer bestätigt; Damenpreise wurden ausdrücklich aktualisiert.
- [x] Mehrwertsteuerangabe vom Nutzer bestätigt.
- [x] Preisformulierungen „ab … bis …“ vom Nutzer bestätigt.
- [x] Wirtschafts-Identifikationsnummer DE413705673 vom Nutzer bestätigt und im Impressum ergänzt.
- [ ] Vorhandensein einer separaten Umsatzsteuer-ID sowie weitere einschlägige Angaben klären; keine persönliche Steuernummer veröffentlichen.

Name Gabriele Zink, Geschäftsanschrift, Handwerkskammer zu Köln, Berufsbezeichnung und Deutschland als Verleihungsland sind bestätigt.

## 4. Hosting vor Testbereitstellung

- Im Host-Europe-Kundenportal die tatsächliche Domainzuordnung zum angegebenen Pfad `/www` prüfen.
- Verschlüsselten Zugang und Port bestimmen: SSH/SFTP oder explizites FTP über TLS. Sichere Anmeldung außerhalb von Projekt, Git und OneDrive; keine Passwörter im Chat.
- Paketkonfiguration für Logs, Verarbeitung, AVV und E-Mail ermitteln, anschließend Datenschutzentwurf ergänzen.
- Zusätzliche Sicherung der alten Website/Serverkonfiguration und Wiederherstellungstest entfallen auf ausdrückliche Nutzerentscheidung. Testbereitstellung nach technischer Vorbereitung zur Freigabe vorlegen; bestehende Mail- und DNS-Konfiguration erhalten.

Weiterleitungen und Umschaltung folgen den getrennten Plänen in `WEITERLEITUNGEN.md` und `ROLLOUT.md`.
