# Offene Punkte und Entscheidungen

Stand: 11.10.2026

## Bestandsaufnahme

- [x] Verbindliches Arbeitsverzeichnis geprüft: ursprünglich leer, kein Repository im Verzeichnis oder in Elternverzeichnissen, keine geltenden AGENTS.md gefunden.
- [x] Bestehenden Sites-Eintrag über Eigentümerzugriff identifiziert; Quellcode und zwei ursprüngliche Git-Commits direkt ins Arbeitsverzeichnis übernommen. Kein verschachteltes Repository.
- [x] HTML/CSS, Originalfoto, vorhandene README und Sites-Zuordnung eingesehen. Website-Dateien unverändert erhalten.
- [x] Telefon, E-Mail, Einsatzgebiet und Terminzeiten mit bisheriger öffentlicher Startseite abgeglichen; noch keine Aktualitätsbestätigung durch Gaby.
- [x] Projektregeln, Vorschauhinweise und Roll-out-Plan dokumentiert. Keine Veröffentlichung und keine DNS-/Hosting-Änderung.

## Anpassungen auf Nutzeranweisung

- [x] Damenpreise nach neuer Nutzertabelle aktualisiert, „Eindrehen“ entfernt und alle 15 Positionen mit der Vorgabe abgeglichen.

- [x] Foto-Schriftzug „Deine Friseurin“ entfernt.
- [x] Haarverlängerung inklusive Beratungsschaltfläche und Erwähnungen in Seitenbeschreibungen entfernt; Leistungsnummerierung und Desktop-Raster auf drei Angebote angepasst.
- [x] Dauerwelle aus der Preisliste entfernt.
- [x] Terminzeit auf Montag bis Freitag 10:00–17:00 Uhr geändert; „und auf Anfrage“ beibehalten.
- [x] Quelltext, lokale Linkziele und Git-Diff geprüft; visuelle Browserprüfung steht noch aus.

## Nächste Arbeit und offene Entscheidungen

- [ ] Lokale Vorschau läuft unter http://127.0.0.1:8000/; Desktop und Smartphone sowie Tastatur, Kontraste, Preislisten, Bilder, Kontaktlinks, Metadaten und interne Links prüfen. Noch keine Browserprüfung durchgeführt.
- [ ] Gaby bestätigt Kontaktdaten, Terminzeiten, Preise, Qualifikation seit 2009 sowie Produkt-/Markenangaben und Fotoverwendung.
- [ ] Impressum: vollständiger Anbietername, Geschäftsanschrift, tatsächliche Kammerzugehörigkeit, Verleihungsland und gegebenenfalls erforderliche Identifikationsnummern klären. Übernommene Annahmen nicht als bestätigt behandeln.
- [ ] Bisherigen Hosting-Anbieter, sicheren Zugriff, Dokumentwurzel, Servertechnik, Protokollierung/Log-Aufbewahrung und E-Mail-Betrieb klären. Keine Zugangsdaten hier eintragen.
- [ ] Eigene Datenschutzseite anhand tatsächlicher Technik und Hosting-Angaben vorbereiten und prüfen lassen; alten Datenschutzlink anschließend passend ersetzen.
- [ ] Alte URLs vollständig inventarisieren. Vorläufige Zuordnung prüfen: `/phil.html` → `/#gaby`; `/d.html`, `/h.html`, `/k.html`, `/div.html` → `/#preise`; `/s-b.html`, `/braut.html` → `/#leistungen`; Ziel für `/hvl.html` nach Entfernung des Angebots gesondert abstimmen; `/dgsvo.html` → künftige eigene Datenschutzseite. Kategoriegenaue Anker bei Bedarf ergänzen. Weiterleitungen erst nach bestätigter URL-Liste und Servertechnik implementieren.
- [ ] Sicherung und Wiederherstellung der alten Website vorbereiten; Testbereitstellung, Umschaltplan und Rückfallweg konkretisieren. E-Mail-Konfiguration erhalten.
- [ ] Testbereitstellung und spätere Umschaltung jeweils ausdrücklich freigeben lassen; danach Funktionsprüfung inklusive E-Mail durchführen.

Entschieden: vorhandene HTML/CSS-Lösung und Bordeaux-Design weiterverwenden; zunächst bisheriges Hosting anstreben. Keine neue Website-Variante, keine zusätzlichen Abhängigkeiten und keine Veröffentlichung bei dieser Bestandsaufnahme.

## Fotoexperiment (noch nicht übernommen)

- Ausgangsstand inklusive Damenpreise auf `main` in Commit `111b3ca` gesichert.
- Branch: `experiment/gaby-entspannter`. Variante `dist/assets/gaby-entspannt.png` mit integriertem Imagegen erstellt und lokal eingebunden; Original `dist/assets/gaby.jpg` bleibt erhalten.
- Entscheidung zur Übernahme offen. Zurück zum bisherigen Stand: nach Sicherung des Experiments `git switch main`. Kein Push und keine Veröffentlichung.
- Prompt und Herkunft: `FOTO-EXPERIMENT.md`.
