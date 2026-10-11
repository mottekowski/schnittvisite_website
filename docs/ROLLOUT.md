# Roll-out bei Host Europe

Stand: 11.10.2026. Hoster Host Europe, Paket „WebHosting Basic [WebHosting 2016 Basic]“ und Webspace-Pfad `/www` vom Nutzer angegeben. Zunächst wurde SFTP, zuletzt FTP genannt; das tatsächlich verfügbare verschlüsselte Protokoll bleibt zu prüfen. Kein Zugang hergestellt, keine Dateien auf dem Server geändert und keine Testbereitstellung veröffentlicht.

## 1. Voraussetzung und Freigaben

- Angegebenes Paket: WebHosting 2016 Basic. Angegebener Pfad: `/www`; die tatsächliche Domainzuordnung im Kundenportal beziehungsweise Serverbestand verifizieren. Webserver, verschlüsseltes Protokoll und Port prüfen. Serveradresse nur aus dem Chat beziehungsweise sicherer Sitzung verwenden; keine Verbindungsdaten im Projekt hinterlegen.
- SFTP-Anmeldedaten über einen sicheren Zugang außerhalb von Git und OneDrive verwenden. Hostschlüssel über eine unabhängige Quelle prüfen. Keine Passwörter in Skripte oder Projektdateien eintragen.
- Exakte Namensschreibweise und offene Berufsangaben bestätigen; die Anschrift Dechenstraße 13, 53115 Bonn, Deutschland ist vom Nutzer bestätigt; Datenschutzentwürfe einschließlich Hosting, AVV, E-Mail-Dienst, Fristen und Cookie-Prüfung finalisieren.
- Separate Freigabe für Testbereitstellung einholen. Nach abgeschlossenen Tests genaue Dateiliste, Serverregeln und Umschaltzeitpunkt zur ausdrücklichen Produktionsfreigabe vorlegen.

## 2. Sicherung vor jeder Serveränderung

- Gesamte aktuelle Dokumentwurzel einschließlich versteckter Konfigurationsdateien per SFTP herunterladen. Server-/Domainzuordnung und bestehende Weiterleitungen separat erfassen. Bei vorgefundenem Backend oder Datenbanken diese gesondert sichern.
- Sicherung mit Datum außerhalb des Website-Auslieferungsordners aufbewahren; sensible Konfiguration außerhalb von Git und OneDrive. Dateiliste, Dateigrößen und Prüfsummen erstellen und Stichproben öffnen.
- Provider-Backup und Wiederherstellungsoptionen für das konkrete Paket prüfen. Eine Wiederherstellung in einem getrennten Testverzeichnis erproben. Sicherung erst danach als wiederherstellbar markieren.
- Der öffentliche URL-Abruf in `alte-urls.json` ist keine Website-Sicherung. Die lokale Git-Historie sichert ausschließlich die neue Website.

## 3. E-Mail und DNS erhalten

- Öffentlicher DNS-Abgleich liegt in `dns-vor-rollout.json`. Beobachtet: MX `mx0.schnittvisite.com` (Priorität 50), Nameserver `ns21.domaincontrol.com` und `ns22.domaincontrol.com`. Das belegt weder das Hosting-Paket noch den E-Mail-Vertrag.
- Vollständige DNS-Zone im zuständigen Portal exportieren, einschließlich SPF, DKIM, DMARC, Subdomains und Mail-Serveradressen. Der öffentliche Abgleich ist kein vollständiger Zonenexport.
- Geplant ist ausschließlich der Austausch von Website-Dateien auf dem bisherigen Webspace. Keine Nameserver-, MX- oder sonstigen DNS-Änderungen erforderlich voraussetzen oder durchführen.
- Postfächer und Maildaten nicht in eine Website-Dateisynchronisierung aufnehmen. Vorher und nachher empfangen und senden lassen; E-Mail-Testnachrichten nur mit ausdrücklichem Auftrag versenden.

## 4. Testbereitstellung nach Freigabe

- Getrennte Dokumentwurzel mit Zugriffsschutz und HTTPS verwenden; kein Unterordner, der wegen der absoluten CSS-/Bildpfade die Produktionsdateien lädt. Bestehende Root-Dateien bleiben erhalten.
- Nur referenzierte Website-Dateien ausliefern: `index.html`, `impressum.html`, `datenschutz.html`, `cookie-hinweise.html`, `style.css`, `assets/gaby-entspannt.webp`. Vollständige Referenzprüfung unmittelbar davor wiederholen. Originalbilder bleiben lokal/Git erhalten.
- Keine `.git`, `.openai`, README, TODO, Prüfberichte oder unreferenzierten großen Bildvarianten auf das Ziel übertragen. Freigabe verhindert nicht die Notwendigkeit fertiggestellter rechtlicher Seiten.
- Smartphone/Desktop, echte iOS-/Android-Geräte, Tastatur, alle Preislisten, Bild, Metadaten und Links prüfen. HTTP-Header auf Cookies, Browser auf Speicherzugriffe und Server auf Protokollierung prüfen. Cookie-Namen/Werte mit Zugangs- oder Sitzungstokens nicht in Git dokumentieren.
- Weiterleitungszuordnung aus `WEITERLEITUNGEN.md` auf dem Testserver umsetzen und prüfen. `/hvl.html` zuvor entscheiden.

## 5. Umschaltung nach ausdrücklicher Freigabe

- Getesteten lokalen Commit und Dateiprüfsummen festhalten. Eine aktuelle Sicherung direkt vor dem Wechsel erstellen und Änderungen seit der ersten Sicherung abgleichen.
- Neue Dateien in einem getrennten Verzeichnis vorbereiten; je nach Paket die Domain-Dokumentwurzel kontrolliert umstellen oder einen vom Anbieter unterstützten atomaren Austausch nutzen. Keine pauschale Synchronisierung mit Löschoption.
- Vorhandene Serverregeln behutsam ergänzen; Weiterleitungen erst aktivieren, wenn Ziele erreichbar sind. Dokumentierte E-Mail-/DNS-Konfiguration erhalten.
- Hauptseite, alle rechtlichen Seiten, Preislisten, Bild, HTTPS und jede Alt-URL nach dem Wechsel prüfen. Mail-Senden/-Empfangen gesondert prüfen lassen.

## 6. Rückfall

- Rückfall auslösen bei fehlenden Seiten/Bildern, Weiterleitungsschleifen, SSL-Fehlern, nicht nutzbarem Kontakt oder E-Mail-Störung. Ergebnis und Zeitpunkt festhalten.
- Vorherige Dokumentwurzel wieder zuordnen oder die gesicherten Website-Dateien und Serverregeln wiederherstellen. Keine Maildaten oder DNS-Zone mit einer Website-Sicherung überschreiben.
- Alte Haupt-/Unterseiten, HTTPS und E-Mail erneut prüfen lassen. Neue Dateien für Ursachenanalyse erhalten; keinen ungezielten rekursiven Löschbefehl ausführen.

## Offizielle Hinweise für die Paketprüfung

- [Host Europe: Logdateien und konfigurierbare IP-Anonymisierung](https://www.hosteurope.de/faq/webhosting/webhosting-logfiles/logfiles-einsehen-und-aendern)
- [Host Europe: Backup für WebHosting](https://www.hosteurope.de/faq/webhosting/restore-und-backup)
- [Host Europe: Vertrag zur Auftragsverarbeitung](https://www.hosteurope.de/faq/vertrag-und-rechnungen/vertrag/adv-vertrag)

Diese Dokumentation bestätigt keine konkrete Log-Aufbewahrungsdauer, keinen abgeschlossenen AVV und keinen tatsächlichen Serverstandort des gebuchten Pakets.

[Host Europe: SFTP und FTPES](https://www.hosteurope.de/faq/webhosting/hochladen-von-webinhalten-ftp/ftp-verschluesselt-uebertragen): SFTP verwendet den SSH-Zugang; FTPES ist die TLS-verschlüsselte FTP-Variante. Die richtige Verbindung für dieses Paket muss anhand des Kundenportals geprüft werden.
