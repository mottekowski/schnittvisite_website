# Schnittvisite – Gaby Zink

Statische HTML/CSS-Website, ursprünglich erstellt am 15.09.2026. Am 11.10.2026 wurde der vorhandene Sites-Quellcode samt Git-Historie in das zuvor leere Arbeitsverzeichnis übernommen. Kein Framework, kein Build und keine Paketinstallation erforderlich.

- Arbeitsverzeichnis: `C:\Users\chzin\OneDrive - Schnittvisite\SV\Website`
- Bisherige Website: https://www.schnittvisite.com
- Ausgangsversion in Sites: https://schnittvisite-gaby.mottekowski.chatgpt.site (Zugriff laut Sites auf Eigentümer beschränkt)
- Aktuelle Dateien: `dist/index.html`, `dist/impressum.html`, `dist/datenschutz.html`, `dist/cookie-hinweise.html`, `dist/style.css`, `dist/assets/gaby-entspannt.webp`. Originalfoto und PNG-Variante bleiben zur Nachvollziehbarkeit erhalten.
- Importierter Ausgangscommit: `9d39f06c3bba36683ffec60a0362e41f24188fd0`
- `.openai/hosting.json` ordnet den bestehenden Sites-Eintrag zu; es ist keine Konfiguration des bisherigen Hosting-Anbieters.

## Start und lokale Vorschau

PowerShell im Arbeitsverzeichnis öffnen. Ein vorhandener Python-3-Interpreter kann ohne neue Abhängigkeiten die Vorschau bereitstellen:

```powershell
Set-Location -LiteralPath 'C:\Users\chzin\OneDrive - Schnittvisite\SV\Website'
& 'C:\Users\chzin\.cache\codex-runtimes\codex-primary-runtime\dependencies\python\python.exe' -m http.server 8000 --bind 127.0.0.1 --directory dist
```

Danach `http://127.0.0.1:8000/` im Browser öffnen; mit Strg+C stoppen. Falls `python` nur den Windows-Installationsalias öffnet, einen vorhandenen echten Python-Interpreter verwenden. Die Vorschau läuft und wurde per HTTP und Browser geprüft. Dokumentwurzel muss `dist` sein, da CSS und Bild mit absoluten Website-Pfaden verlinkt sind; direktes Öffnen der HTML-Datei ist dafür ungeeignet.

## Herkunft und Inhalt

Quellen laut übernommener Dokumentation:

- Startseite, Kontakt, Foto: https://www.schnittvisite.com/
- Vorstellung und Qualifikation: https://www.schnittvisite.com/phil.html
- Preise: `/d.html`, `/h.html`, `/k.html`, `/div.html` der bisherigen Website
- Leistungen: `/hvl.html`, `/s-b.html`, `/braut.html` der bisherigen Website
- Bisheriger Datenschutz: https://www.schnittvisite.com/dgsvo.html
- Originalfoto: https://www.schnittvisite.com/images/Gaby_1.jpg (lokal unter `dist/assets/gaby.jpg`)

Telefon 0174 / 344 76 77, E-Mail gaby@schnittvisite.com, Bonn und Umgebung sowie Montag bis Freitag 10:00–18:00 Uhr und auf Anfrage wurden am 11.10.2026 mit der bisherigen öffentlichen Startseite abgeglichen. Die Nutzerfreigabe bestätigt inzwischen Kontaktangaben, Einsatzgebiet, Friseurmeisterin seit 2009, Fotoverwendungsrechte sowie die Herren-, Kinder- und Zusatzpreise einschließlich Mehrwertsteuer. Die Terminzeit wurde anschließend auf Nutzeranweisung auf Montag bis Freitag 10:00–17:00 Uhr und auf Anfrage geändert. Haarverlängerung und Dauerwelle wurden aus dem Angebot der neuen Website entfernt. Damenpreise wurden anschließend nach der neuen Nutzertabelle aktualisiert und „Eindrehen“ entfernt. Preisformulierungen wie „ab … bis …“ wurden vom Nutzer ausdrücklich bestätigt.

Der eingesehene Quellcode enthält keine Skripte, Formulare, Analysewerkzeuge, externen Schriftendienste oder Browserspeicherung. Preislisten verwenden native `details`-Elemente. Hosting kann zusätzliche Zugriffskontrollen und Protokollierung mitbringen.

Das Impressum ist ausdrücklich ein Entwurf. Laut ursprünglicher Dokumentation stammt die Anschrift aus der alten Datenschutzseite; der vollständige Name beruht teilweise auf früherem Nutzerkontext und die Kammerzuordnung wurde aus der Bonner Anschrift abgeleitet. Kammerzugehörigkeit und Berufsbezeichnung wurden inzwischen vom Nutzer bestätigt. Die Anschrift Dechenstraße 13, 53115 Bonn, Deutschland, der vollständige Name Gabriele Zink und Deutschland als Verleihungsland wurden ebenfalls bestätigt. Die Wirtschafts-Identifikationsnummer DE413705673 wurde vom Nutzer bestätigt und im Impressum ergänzt. Weitere gegebenenfalls einschlägige Angaben bleiben abschließend zu prüfen. Eine eigene Datenschutzseite ist nun als sichtbar gekennzeichneter Entwurf verlinkt; der alte Datenschutzlink wurde ersetzt. Hosting- und Verarbeitungsdetails bleiben zu ergänzen.

## Veröffentlichung und Rückfallplan

Host Europe, „WebHosting Basic [WebHosting 2016 Basic]“ und Webspace-Pfad `/www` sind vom Nutzer angegeben. Domainzuordnung, verschlüsseltes Zugangsprotokoll/Port, sicherer Zugang und Weiterleitungsmechanismus bleiben zu prüfen. Der konkrete Ablauf steht in `docs/ROLLOUT.md`. Keine Veröffentlichung, DNS-/Hosting-Änderung oder Ersetzung ohne ausdrückliche Nutzerfreigabe.

1. Hosting und E-Mail-Zuständigkeit klären. Zusätzliche Sicherung, DNS-Zonenexport und Wiederherstellungstest entfallen auf Nutzerentscheidung vom 11.10.2026. Zugangsdaten bleiben außerhalb von Projekt, Git und OneDrive.
2. Alte URLs inventarisieren und passende Weiterleitungen abstimmen. Nach Möglichkeit Domain, Nameserver und Mail-Konfiguration beibehalten; MX, SPF, DKIM und DMARC erhalten; spätere notwendige Änderungen gesondert freigeben lassen.
3. Nach Freigabe der Testbereitstellung Inhalte von `dist` in eine separate Test-Dokumentwurzel übertragen. Testzugang und Suchmaschinenzugriff passend konfigurieren. Rechtliche Seiten und Inhalte bestätigen lassen.
4. Smartphone/Desktop, Tastatur, Kontraste, Navigation, alle Preislisten, Bild, Kontaktlinks, Metadaten und interne Links prüfen. Weiterleitungen und HTTPS auf dem Zielhosting prüfen.
5. Konkreten geprüften Stand und Umschaltplan zur ausdrücklichen Freigabe vorlegen. Nach Freigabe nur Website-Dateien aus `dist` ausliefern, nicht Git, Dokumentation oder `.openai`. DNS nur nach gesonderter ausdrücklicher Freigabe ändern.
6. Direkt danach Haupt-/Unterseiten, Weiterleitungen, HTTPS, Telefon-/E-Mail-Links und bestehenden E-Mail-Betrieb prüfen. Bei Fehlern eine erhalten gebliebene vorherige Dokumentwurzel wieder zuordnen, soweit verfügbar; keine zusätzliche Sicherung voraussetzen.

Offene Punkte und Prüfstatus stehen in `TODO.md`; verbindliche Arbeitsregeln in `AGENTS.md`.

## Freigegebene Fotovariante

Nach Nutzerfreigabe wurde die PNG-Fotovariante übernommen; auf der Startseite ist jetzt ihre optimierte WebP-Fassung `dist/assets/gaby-entspannt.webp` (rund 169 KB) eingebunden. Das Original `dist/assets/gaby.jpg` bleibt erhalten. Herkunft und Prompt stehen in `FOTO-EXPERIMENT.md`. Die Übernahme in `main` ist keine Veröffentlichung.

## Cookie-Hinweise

`dist/cookie-hinweise.html` enthält einen verlinkten Entwurf zu Cookies und ähnlichen Technologien. Der eigene Code nutzt keine Cookies, Analysewerkzeuge oder Browser-Speicherung. Das endgültige Hosting ist noch zu prüfen; deshalb ist dies keine fertige Datenschutzerklärung. Es wurde kein Einwilligungsbanner ergänzt. Die Entwurfsseite enthält `noindex`, das bei einer späteren Finalisierung erneut zu beurteilen ist.

## Prüfstand und Veröffentlichung

`docs/PRUEFBERICHT.md` dokumentiert lokale Browser-, Tastatur-, Kontrast- und Linkprüfungen. `docs/WEITERLEITUNGEN.md` enthält die 11 öffentlich erreichbaren Alt-URLs mit Zielzuordnung; unbekannte Serverdateien bleiben zu erfassen. `docs/ROLLOUT.md` beschreibt Testbereitstellung, Umschaltung und verfügbare Rückfallmöglichkeiten bei Host Europe sowie den ausdrücklich abgewählten Sicherungsschritt. Rechtliche Texte sind noch Entwürfe; kein Upload, Push oder DNS-Wechsel wurde durchgeführt. Für den Roll-out nur die im Roll-out-Dokument genannten referenzierten Dateien übertragen, nicht den gesamten Projektordner.

## Favicon

`dist/favicon.ico` ist das vom Nutzer bereitgestellte Original-Icon und auf allen vier HTML-Seiten als Tab-Symbol verlinkt. Bei Veröffentlichung zusammen mit den übrigen referenzierten Dateien ausliefern.

## Veröffentlichung am 11.10.2026

Auf ausdrücklichen Nutzerauftrag wurden die sieben referenzierten Dateien aus Commit f1e9c33 auf den bisherigen Host-Europe-Webspace übertragen. Die vorhandene FileZilla-Verbindung wurde per FTPES mit Zertifikatsprüfung verwendet; keine Zugangsdaten in Projekt, Git oder zusätzlichen Dateien gespeichert. Beide Domainvarianten wurden vorab durch eine temporäre Testdatei der FTP-Dokumentwurzel zugeordnet; die Testdatei wurde entfernt. Der FTP-Zugang ist auf die Dokumentwurzel eingeschränkt, daher ist /www nicht als Unterverzeichnis erreichbar.

Alle sieben veröffentlichten Dateien: HTTP 200, SHA-256 identisch zum lokalen Stand, kein Set-Cookie-Header beobachtet. Startseite im Browser bei 1280 und 390 Pixeln ohne horizontalen Überlauf; Foto geladen, Favicon verlinkt, Herrenpreisliste erfolgreich geöffnet. DNS und E-Mail-Konfiguration wurden nicht geändert; keine E-Mail-Testnachricht versandt. Zusätzliche Sicherung entfiel gemäß Nutzerentscheidung. Rechtliche Seiten bleiben sichtbar gekennzeichnete Entwürfe. Alte URL-Weiterleitungen, tatsächliche Hosting-/Datenschutzdetails und echte Geräteprüfungen bleiben offen.

## Cookie-Prüfung vom 11.10.2026

- [x] Alle sieben aktiven Live-Dateien über HTTPS geprüft: HTTP 200, kein Set-Cookie-Header. Live-DOM der Cookie-Seite ohne Skripte, Frames oder externe Ressourcen; Quellcode ohne Tracking, Formulare, Cookies oder Web Storage.
- [x] Cookie-Hinweise lokal aus dem Entwurfsmodus genommen; Beschreibung, Text und Footer-Verweise auf allen vier Seiten angepasst. noindex auf der Cookie-Seite entfernt.
- [x] Datenschutztext auf tatsächlich betriebenes Host-Europe-Hosting aktualisiert und Cookie-Prüfung übernommen. Datenschutz bleibt Entwurf: Nutzer meldet AVV, E-Mail-Anbieter und Log-Einstellungen als unbekannt. Keine Angaben dazu erfunden.
- [ ] Tatsächliche Hosting-/E-Mail-Verarbeitung bestätigen und Datenschutz anschließend fertigstellen. Nach Host-Europe-FAQ im KIS unter Produktverwaltung > WebHosting > Konfigurieren > Statistiken & Logfiles die Log-Konfiguration prüfen; Vertragsstatus separat bestätigen.
- [x] Änderungen dieser Prüfung auf ausdrücklichen Deploy-Auftrag am 11.10.2026 veröffentlicht. Vier HTML-Dateien übertragen; alle sieben aktiven Dateien öffentlich per HTTPS/HTTP 200 und SHA-256 geprüft. Datenschutz weiterhin Entwurf. Noch kein Git-Push für diese Änderung.

Für die fehlenden Betriebsangaben zur Datenschutzerklärung: ausfüllbare Checkliste in docs/DATENSCHUTZ-CHECKLISTE.md. Antworten mit Quelle/Datum ergänzen; keine Zugangsdaten oder Kundendaten eintragen.
