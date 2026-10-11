# Offene Punkte und Entscheidungen

Stand: 11.10.2026. Die Website wurde nach ausdrücklicher Nutzerfreigabe am 11.10.2026 auf dem bestehenden Host-Europe-Webspace veröffentlicht. Rechtliche Entwürfe und weitere unten genannte Punkte bleiben offen.

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
- [x] Konkrete Abnahmeliste für echte Geräte, weitere Barrierefreiheitsprüfungen, Inhaltsfreigabe und Hosting-Voraussetzungen vorbereitet: docs/ABNAHME.md. Die lokale Loopback-Vorschau ist auf Handys nicht erreichbar; keine Netzwerkfreigabe eingerichtet.

## 2. Inhalt bestätigen

- [x] Nutzer bestätigt Host Europe, Zugangsart SFTP, Handwerkskammer zu Köln, Friseurmeisterin sowie Goldwell und Alterna. Beide Produktmarken sind genannt.
- [x] Nutzer bestätigt Telefon 0174 / 344 76 77, gaby@schnittvisite.com, Bonn und Umgebung, Friseurmeisterin seit 2009, Fotoverwendungsrechte sowie aktuelle Herren-/Kinder-/Zusatzpreise. Damenpreise und geänderte Terminzeiten wurden bereits ausdrücklich vorgegeben.
- [x] Preise einschließlich Mehrwertsteuer vom Nutzer bestätigt.
- [x] Preisformulierungen „ab … bis …“ vom Nutzer ausdrücklich bestätigt.

## 3. Impressum

- [x] Geschäftsanschrift vom Nutzer bestätigt: Dechenstraße 13, 53115 Bonn, Deutschland.
- [x] Vollständiger Anbietername vom Nutzer bestätigt: Gabriele Zink. In Impressum und Datenschutzentwurf übernommen.
- [x] Verleihungsland der Berufsbezeichnung vom Nutzer bestätigt: Deutschland. Im Impressum ergänzt.
- [x] Wirtschafts-Identifikationsnummer DE413705673 vom Nutzer bestätigt und im Impressum eingetragen.
- [ ] Vorhandensein einer separaten Umsatzsteuer-ID sowie gegebenenfalls weitere einschlägige Angaben klären. Die Wirtschafts-ID ist keine Bestätigung einer Umsatzsteuer-ID.
- [x] Kammerzugehörigkeit und Berufsbezeichnung laut Nutzer bestätigt; Impressum weiterhin deutlich als Entwurf behandelt und mit eigener Beschreibung/noindex versehen.

## 4. Hosting und Datenschutz

- [x] Paket „WebHosting Basic [WebHosting 2016 Basic]“ und Webspace-Pfad `/www` vom Nutzer angegeben. Serveradresse liegt im Chat vor; keine Verbindungsdaten in Projektdateien gespeichert.
- [x] FTPES mit Zertifikatsprüfung und Domainzuordnung bestätigt: kurzzeitige Testdatei unter beiden Domainvarianten erreichbar und wieder entfernt. Der FTP-Zugang zeigt direkt die Dokumentwurzel; /www ist darin kein Unterverzeichnis. Zugang aus der vorhandenen FileZilla-Konfiguration ausschließlich im Prozessspeicher genutzt.
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
- Entfällt auf ausdrückliche Nutzerentscheidung: zusätzliche Website-/Serverkonfigurationssicherung und Wiederherstellungstest. Kein Backup als durchgeführt markieren.
- Entfällt auf Nutzerentscheidung: zusätzlicher vollständiger DNS-Zonenexport.
- [ ] E-Mail-Anbieter klären und bestehenden Mailbetrieb vor/nach Umschaltung prüfen lassen; Mail- und DNS-Konfiguration erhalten.
- [ ] Testbereitstellung ausdrücklich freigeben lassen; auf Zielhosting technische und rechtliche Endprüfung durchführen.
- [x] Produktionsfreigabe durch Nutzerauftrag zum Deployen erhalten. Sieben referenzierte Dateien aus Commit f1e9c33 veröffentlicht; alle öffentlich per HTTPS/HTTP 200 und SHA-256-Abgleich geprüft. DNS/E-Mail unverändert. Weiterleitungen sind weiterhin offen.

Website am 11.10.2026 veröffentlicht; keine DNS-/E-Mail-Änderung und kein Push. Die offene Workspace-Datei schnitvisite_website.code-workspace bleibt unverändert.

## Favicon und Zugangstest

- [x] Nutzer meldet erfolgreiche Verbindung mit FileZilla. Konkretes Protokoll/TLS, Domainzuordnung und Serverkonfiguration sind damit noch nicht unabhängig geprüft.
- [x] Vorhandene ICO-Datei unverändert nach `dist/favicon.ico` kopiert und als Tab-Icon auf allen vier HTML-Seiten eingebunden.

## Cookie-Prüfung vom 11.10.2026

- [x] Alle sieben aktiven Live-Dateien über HTTPS geprüft: HTTP 200, kein Set-Cookie-Header. Live-DOM der Cookie-Seite ohne Skripte, Frames oder externe Ressourcen; Quellcode ohne Tracking, Formulare, Cookies oder Web Storage.
- [x] Cookie-Hinweise lokal aus dem Entwurfsmodus genommen; Beschreibung, Text und Footer-Verweise auf allen vier Seiten angepasst. noindex auf der Cookie-Seite entfernt.
- [x] Datenschutztext auf tatsächlich betriebenes Host-Europe-Hosting aktualisiert und Cookie-Prüfung übernommen. Datenschutz bleibt Entwurf: Nutzer meldet AVV, E-Mail-Anbieter und Log-Einstellungen als unbekannt. Keine Angaben dazu erfunden.
- [ ] Tatsächliche Hosting-/E-Mail-Verarbeitung bestätigen und Datenschutz anschließend fertigstellen. Nach Host-Europe-FAQ im KIS unter Produktverwaltung > WebHosting > Konfigurieren > Statistiken & Logfiles die Log-Konfiguration prüfen; Vertragsstatus separat bestätigen.
- [x] Änderungen dieser Prüfung auf ausdrücklichen Deploy-Auftrag am 11.10.2026 veröffentlicht. Vier HTML-Dateien übertragen; alle sieben aktiven Dateien öffentlich per HTTPS/HTTP 200 und SHA-256 geprüft. Datenschutz weiterhin Entwurf. Noch kein Git-Push für diese Änderung.

## Herrenpreise vom 11.10.2026

- [x] Nutzertabelle übernommen: Cut & Leave 30 €, Waschen/Schnitt/Föhnen 35 €, Neuschnitt 45 €, Kopfmassage auf Anfrage, Färben/Tönen je 50 €, Kammsträhnen 45 €, Barttrimmen 20 €; alle Beträge mit vorgegebenem Zusatz „ab“.
- [x] Neue Herrenpreise nach ausdrücklichem Deploy-Auftrag am 11.10.2026 veröffentlicht. Beide Domainvarianten: HTTPS/HTTP 200, Datei per SHA-256 identisch und alle acht Herrenpreise korrekt.
