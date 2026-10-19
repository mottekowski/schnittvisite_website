# Weiterleitungen: lokaler Implementierungsstand

Stand: 19.10.2026. Die Regeln sind lokal in `dist/.htaccess` vorbereitet, aber noch nicht auf den Webserver übertragen oder auf einem Testziel geprüft.

Über alle gefundenen internen HTML-Links der alten Startseite wurden 11 URLs erreicht und mit HTTP 200 geprüft. Details: `alte-urls.json`. Unverlinkte Seiten, Suchmaschinen-URLs und Serverdateien können nur mit Hosting-Dateiliste und gegebenenfalls Suchkonsole/Zugriffsprotokollen vollständig erfasst werden.

| Alter Pfad | Neues Ziel | Status |
| --- | --- | --- |
| `/` | `/` | Startseite bleibt |
| `/index.html` | `/` | 301 lokal vorbereitet |
| `/phil.html` | `/#gaby` | 301 lokal vorbereitet |
| `/d.html` | `/#preise-damen` | 301 lokal vorbereitet |
| `/h.html` | `/#preise-herren` | 301 lokal vorbereitet |
| `/k.html` | `/#preise-kinder` | 301 lokal vorbereitet |
| `/div.html` | `/#preise-extra` | 301 lokal vorbereitet |
| `/s-b.html` | `/#farbe-balayage` | 301 lokal vorbereitet |
| `/braut.html` | `/#brautfrisuren` | 301 lokal vorbereitet |
| `/dgsvo.html` | `/datenschutz.html` | 301 lokal vorbereitet |
| `/hvl.html` | Kein Ziel | 410 lokal vorbereitet; Angebot wurde entfernt und kein passender Ersatzinhalt ist vorhanden |

Die Zielanker sind im HTML vorhanden. Preisanker führen zur jeweiligen aufklappbaren Kategorie; es ist keine automatische Öffnung per JavaScript eingebaut. Nutzer können die Liste direkt öffnen.

Die Regeln setzen Apache `mod_rewrite` voraus, wie bei Host Europe vorgesehen. Vor einer Übertragung auf ein freigegebenes Testziel HTTP-Status, Location, Zielanker, Schleifen und Parameterverhalten prüfen. Unbekannte Alt-URLs nicht pauschal auf die Startseite umleiten.
