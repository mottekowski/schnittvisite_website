# Lokaler Prüfbericht

Stand: 11.10.2026, lokale HTTP-Vorschau. Keine Produktionsfreigabe.

## Durchgeführte Prüfung

- Startseite, Impressum, Cookie-Hinweise und Datenschutz bei 320, 390, 768 und 1440 Pixeln im Browser: Dokumentbreite entspricht verfügbarer Inhaltsbreite, kein horizontales Überlaufen. Bild geladen.
- Hauptüberschrift bei 320 Pixeln nach Verkleinerung visuell geprüft: die drei vorgesehenen Zeilen passen. Screenshot: `mobil-320.png`.
- Startseite mit Tab durchlaufen: Navigation, Leistungslinks, vier Preislisten, Kontakt- und Footerlinks erreichbar; alle geprüften interaktiven Elemente mit sichtbarem 3-Pixel-Fokus. Nach dem letzten Link wechselt der Fokus regulär in die Browseroberfläche.
- Alle vier Preislisten mit Leertaste geöffnet/geschlossen; Herrenliste zuvor mit Enter geprüft. Inhalte weiterhin native HTML-Tabellen mit Zeilenüberschriften.
- Sprunglink „Zum Inhalt“ per Enter geprüft: URL `#inhalt` und Fokus auf `main#inhalt`. `tabindex="-1"` ermöglicht das ohne zusätzlichen Tab-Stopp.
- Textkontraste auf der Startseite aus berechneten Farben gegen solide Hintergrundflächen geprüft. Bei 320 Pixeln kleinster gemessener Wert rund 5,21:1, keine Werte unter 4,5:1. Text über dem Foto separat visuell auf dem dunklen Verlauf beurteilt; dafür keine allgemeine rechnerische Garantie.
- Fokusdarstellung mit Bordeaux- und hellem Ring für helle sowie dunkle Flächen verbessert. Kein vollständiger automatischer WCAG-Konformitätsnachweis.
- Lokale Dateiverweise/Anker, eindeutige IDs, je ein H1 und vorhandene Seitenbeschreibungen geprüft. Rechtliche Entwürfe enthalten `noindex`; diese Markierung bei Finalisierung beurteilen.
- Alle vier HTML-Seiten und WebP-Bild mit HTTP 200 erreichbar. Lokaler Vorschau-Server setzt bei den geprüften HTML-Antworten keinen Set-Cookie-Header. Das ist keine Prüfung des Host-Europe-Hostings.
- Foto ohne neue Bildgenerierung nach WebP umgewandelt: gleiche Auflösung 1085 × 1449, 168.638 statt 2.477.391 Bytes, rund 93,2 % kleiner. Original und freigegebene PNG-Variante bleiben erhalten.
- Goldwell und Alterna gemäß Nutzerangabe genannt. Keine anderen offenen Geschäfts- oder Preisangaben als bestätigt markiert.

## Noch zu prüfen

- Echte iOS-/Android-Geräte: Touch, Browserzoom, Querformat, Preislisten und Telefon-/E-Mail-Übergabe. Kein echtes Mobilgerät in dieser Prüfung verwendet.
- Screenreader und weitere Browser; insbesondere die Wirkung des Sprunglinks außerhalb des verwendeten Browsers. Vollständige Barrierefreiheit ist nicht bestätigt.
- Host-Europe-Paket und Testserver: HTTPS, Cookie-/Speicherzugriffe, Log-Konfiguration, konkrete Weiterleitungen, 404/410-Verhalten und Mailbetrieb.
- Juristische/inhaltsbezogene Bestätigung der im Datenschutz und Impressum sichtbaren offenen Stellen.

## Grundlagen für die Datenschutzvorbereitung

- [DSGVO: insbesondere Art. 13 sowie Art. 15–22](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=CELEX:32016R0679)
- [§ 25 TDDDG](https://www.gesetze-im-internet.de/ttdsg/__25.html)
- [Host Europe: konfigurierbares Log-Verhalten](https://www.hosteurope.de/faq/webhosting/webhosting-logfiles/logfiles-einsehen-und-aendern)

Die konkrete Erklärung bleibt ein Entwurf, weil technische und organisatorische Angaben des gebuchten Pakets noch fehlen.
