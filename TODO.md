# Offene Punkte und Entscheidungen

Stand: 11.10.2026. Die lokalen Arbeitsschritte sind durchgeführt; Veröffentlichung bleibt gesperrt bis zur ausdrücklichen Freigabe und Klärung der offenen Angaben.

## Erledigte Grundlage

- [x] Leeres verbindliches Arbeitsverzeichnis geprüft; bestehenden Sites-Quellcode und Git-Historie übernommen, kein verschachteltes Repository. AGENTS.md und README.md erstellt beziehungsweise ergänzt.
- [x] Foto-Schriftzug entfernt; Haarverlängerung und Dauerwelle entfernt; Terminzeit Montag–Freitag 10:00–17:00 Uhr und auf Anfrage übernommen.
- [x] Neue Damenpreise nach Nutzertabelle übernommen; Eindrehen entfernt.
- [x] Fotovariante separat erprobt und nach Nutzerfreigabe in main übernommen. Originalbild und PNG bleiben erhalten. Prompt: FOTO-EXPERIMENT.md.
- [x] Gemeinsame Startseite als sinnvoll geprüft; rechtliche Inhalte auf getrennten Seiten.

## 1. Qualität und mobile Darstellung

- [x] Alle vier Seiten bei 320, 390, 768 und 1440 Pixeln geprüft; keine horizontalen Überläufe. Foto lädt; 56 lokale Referenzen einschließlich Ankern geprüft. Details: docs/PRUEFBERICHT.md.
- [x] Tastaturpfad der Startseite und alle vier Preislisten geprüft; Sprunglink setzt jetzt den Fokus auf den Inhalt. Kontrast auf soliden Flächen geprüft; Fokus für helle/dunkle Flächen verbessert.
- [x] Kleine mobile Hauptüberschrift angepasst und bei 320 Pixeln visuell geprüft.
- [x] Foto ohne neue Generierung auf WebP optimiert: 168.638 statt 2.477.391 Bytes bei gleicher Auflösung; etwa 93,2 % weniger. Original bleibt erhalten.
- [ ] Echte iOS-/Android-Geräte einschließlich Touch, Zoom, Querformat und Übergabe an Telefon-/E-Mail-App prüfen. Derzeit nur simulierte Browserbreiten geprüft.
- [ ] Screenreader und weitere Browser sowie abschließende Barrierefreiheitsprüfung ergänzen.

## 2. Inhalt bestätigen

- [x] Nutzer bestätigt Host Europe, Zugangsart SFTP, Handwerkskammer zu Köln, Friseurmeisterin sowie Goldwell und Alterna. Beide Produktmarken sind genannt.
- [ ] Aktualität von Telefon/E-Mail/Einsatzgebiet, Herren-/Kinder-/Zusatzpreisen, Qualifikation seit 2009 und Fotoverwendungsrechten bestätigen. Damenpreise und geänderte Terminzeiten wurden ausdrücklich vorgegeben; übrige Preise nicht pauschal als bestätigt markieren.
- [ ] Formulierungen „ab … bis …“ sowie Steuerangabe mit Gaby abschließend abstimmen.

## 3. Impressum

- [x] Geschäftsanschrift vom Nutzer bestätigt: Dechenstraße 13, 53115 Bonn, Deutschland.
- [x] Vollständiger Anbietername vom Nutzer bestätigt: Gabriele Zink. In Impressum und Datenschutzentwurf übernommen.
- [x] Verleihungsland der Berufsbezeichnung vom Nutzer bestätigt: Deutschland. Im Impressum ergänzt.
- [ ] Gegebenenfalls erforderliche USt-/Wirtschafts-ID oder weitere einschlägige Angaben klären.
- [x] Kammerzugehörigkeit und Berufsbezeichnung laut Nutzer bestätigt; Impressum weiterhin deutlich als Entwurf behandelt und mit eigener Beschreibung/noindex versehen.

## 4. Hosting und Datenschutz

- [x] Paket „WebHosting Basic [WebHosting 2016 Basic]“ und Webspace-Pfad `/www` vom Nutzer angegeben. Serveradresse liegt im Chat vor; keine Verbindungsdaten in Projektdateien gespeichert.
- [ ] Domainzuordnung zu `/www`, Webserver und verschlüsseltes Übertragungsprotokoll/Port prüfen. Zunächst SFTP, zuletzt FTP genannt; FTP- und SSH/SFTP-Zugang nicht gleichsetzen. Sicheren Zugang außerhalb von Projekt/Git/OneDrive bereitstellen.
- [ ] Paketkonfiguration prüfen: Log-Datenarten/Fristen, Verarbeitungsort, AVV, Unterauftragnehmer, mögliche Drittlandübermittlungen, Cookie-/Speicherzugriffe und E-Mail-Anbieter. Öffentliche Provider-Dokumentation belegt keine individuellen Einstellungen.
- [x] Eigene Datenschutzseite mit Cookie-Abschnitt als gekennzeichneten Entwurf vorbereitet und im Footer verlinkt; alten Datenschutzlink ersetzt. Keine Speicherfristen oder abgeschlossenen Verträge erfunden.
- [x] Cookie-Hinweise verlinkt. Lokal keine Set-Cookie-Header beobachtet; Website-Code enthält keine Skripte, Analysewerkzeuge, Formulare oder Browser-Speicherung. Keine Aussage über ungeprüftes Zielhosting.
- [ ] Datenschutz/Impressum nach Ergänzung der bestätigten Angaben abschließend prüfen; Entwurfskennzeichnung/noindex erst bei Finalisierung beurteilen. Cookie-Einwilligung nur bei tatsächlichem Bedarf implementieren.

## 5. Alte URLs und Weiterleitungen

- [x] 11 über öffentliche HTML-Links erreichbare URLs geprüft und dokumentiert: docs/alte-urls.json. Zielzuordnung und Kategorie-/Leistungsanker vorbereitet: docs/WEITERLEITUNGEN.md.
- [ ] Inventur mit tatsächlicher Hosting-Dateiliste ergänzen; öffentliche Linkinventur ist nicht vollständig für unverlinkte Dateien.
- [ ] Für entfernte Haarverlängerung /hvl.html zwischen 410 und sachlich passendem Ziel entscheiden.
- [ ] Weiterleitungsregeln nach Serverklärung auf freigegebenem Testziel implementieren und prüfen. Datenschutz-Weiterleitung erst nach Fertigstellung des Textes aktivieren.

## 6. Sicherung, Testbereitstellung und Roll-out

- [x] Host-Europe-Ablauf mit Dokumentwurzel, SFTP, Sicherung, Wiederherstellung, Testbereitstellung, Umschaltung und Rückfall konkretisiert: docs/ROLLOUT.md.
- [x] Öffentlichen DNS-Zustand read-only erfasst: docs/dns-vor-rollout.json. MX und Nameserver dokumentiert; keine DNS-Änderung. Das ist kein vollständiger Zonenexport.
- [ ] Vollständige Website- und Serverkonfigurationssicherung erstellen und Wiederherstellung in getrenntem Ziel prüfen; benötigt Hosting-Zugang. Gegebenenfalls Backend/Datenbanken sichern, falls vorgefunden.
- [ ] Vollständige DNS-Zone einschließlich Mail-Einträgen sichern, E-Mail-Anbieter klären und bestehenden Mailbetrieb vor/nach Umschaltung prüfen lassen.
- [ ] Testbereitstellung ausdrücklich freigeben lassen; auf Zielhosting technische und rechtliche Endprüfung durchführen.
- [ ] Geprüften Commit, Dateiliste, Weiterleitungen und Umschaltzeitpunkt vorlegen; ausdrückliche Produktionsfreigabe einholen. Danach umschalten, Funktionsprüfung durchführen und Rückfallbereitschaft erhalten.

Keine Website veröffentlicht, keine Hosting-/DNS-Änderung und kein Push. Die offene Workspace-Datei schnitvisite_website.code-workspace bleibt unverändert.
