# Weiterleitungen: Vorbereitung

Stand: 11.10.2026. Nur geplant, keine Serverkonfiguration installiert.

Über alle gefundenen internen HTML-Links der alten Startseite wurden 11 URLs erreicht und mit HTTP 200 geprüft. Details: `alte-urls.json`. Unverlinkte Seiten, Suchmaschinen-URLs und Serverdateien können nur mit Hosting-Dateiliste und gegebenenfalls Suchkonsole/Zugriffsprotokollen vollständig erfasst werden.

| Alter Pfad | Neues Ziel | Status |
| --- | --- | --- |
| `/` | `/` | Startseite bleibt |
| `/index.html` | `/index.html` | Startseite bleibt; Canonical-Weiterleitung optional nach Serverprüfung |
| `/phil.html` | `/#gaby` | 301 vorbereitet als Zuordnung |
| `/d.html` | `/#preise-damen` | 301 vorbereitet als Zuordnung |
| `/h.html` | `/#preise-herren` | 301 vorbereitet als Zuordnung |
| `/k.html` | `/#preise-kinder` | 301 vorbereitet als Zuordnung |
| `/div.html` | `/#preise-extra` | 301 vorbereitet als Zuordnung |
| `/s-b.html` | `/#farbe-balayage` | 301 vorbereitet als Zuordnung |
| `/braut.html` | `/#brautfrisuren` | 301 vorbereitet als Zuordnung |
| `/dgsvo.html` | `/datenschutz.html` | Erst nach fertiggestelltem Datenschutztext |
| `/hvl.html` | Noch offen | Angebot entfernt; 410 oder anderes sachlich passendes Ziel abstimmen |

Die Zielanker sind im HTML vorhanden. Preisanker führen zur jeweiligen aufklappbaren Kategorie; es ist keine automatische Öffnung per JavaScript eingebaut. Nutzer können die Liste direkt öffnen.

Die endgültigen Regeln hängen vom Host-Europe-Paket und Webserver ab. Keine ungeprüfte `.htaccess` ausliefern. Vor Aktivierung vorhandene Regeln sichern und Weiterleitungen auf einem freigegebenen Testziel auf HTTP-Status, Location, Zielanker, Schleifen und Parameterverhalten prüfen. Unbekannte Alt-URLs nicht pauschal auf die Startseite umleiten.
