# Roll-out bei Host Europe

Stand: 11.10.2026. Hoster Host Europe, Paket „WebHosting Basic [WebHosting 2016 Basic]“ und Webspace-Pfad `/www` vom Nutzer angegeben. Zunächst wurde SFTP, zuletzt FTP genannt; das tatsächlich verfügbare verschlüsselte Protokoll bleibt zu prüfen. Kein Zugang hergestellt, keine Dateien auf dem Server geändert und keine Testbereitstellung veröffentlicht.

## 1. Voraussetzung und Freigaben

- Angegebenes Paket: WebHosting 2016 Basic. Angegebener Pfad: `/www`; die tatsächliche Domainzuordnung im Kundenportal beziehungsweise Serverbestand verifizieren. Webserver, verschlüsseltes Protokoll und Port prüfen. Serveradresse nur aus dem Chat beziehungsweise sicherer Sitzung verwenden; keine Verbindungsdaten im Projekt hinterlegen.
- SFTP-Anmeldedaten über einen sicheren Zugang außerhalb von Git und OneDrive verwenden. Hostschlüssel über eine unabhängige Quelle prüfen. Keine Passwörter in Skripte oder Projektdateien eintragen.
- Gabriele Zink, Dechenstraße 13, 53115 Bonn, Deutschland sowie Deutschland als Verleihungsland und Handwerkskammer zu Köln sind vom Nutzer bestätigt. Die Wirtschafts-Identifikationsnummer ist bestätigt und im Impressum eingetragen. Weitere gegebenenfalls einschlägige Angaben abschließend prüfen; Datenschutzentwürfe einschließlich Hosting, AVV, E-Mail-Dienst, Fristen und Cookie-Prüfung finalisieren.
- Separate Freigabe für Testbereitstellung einholen. Nach abgeschlossenen Tests genaue Dateiliste, Serverregeln und Umschaltzeitpunkt zur ausdrücklichen Produktionsfreigabe vorlegen.

## 2. Nutzerentscheidung zur Sicherung

Am 11.10.2026 hat der Nutzer die zusätzliche Sicherung der alten Website und Serverkonfiguration, den Wiederherstellungstest und den zusätzlichen DNS-Zonenexport als nicht nötig abgewählt. Diese Schritte sind keine Voraussetzung mehr und wurden nicht durchgeführt. Vorhandene Dateien und Sicherungen nicht ungefragt löschen. Die lokale Git-Historie enthält die neue Website.

## 3. E-Mail und DNS erhalten

- Öffentlicher DNS-Abgleich liegt in `dns-vor-rollout.json`. Beobachtet: MX `mx0.schnittvisite.com` (Priorität 50), Nameserver `ns21.domaincontrol.com` und `ns22.domaincontrol.com`. Das belegt weder das Hosting-Paket noch den E-Mail-Vertrag.
- Kein zusätzlicher DNS-Zonenexport gemäß Nutzerentscheidung. Bestehende SPF-, DKIM-, DMARC-, Nameserver- und MX-Einstellungen erhalten.
- Geplant ist ausschließlich der Austausch von Website-Dateien auf dem bisherigen Webspace. Keine Nameserver-, MX- oder sonstigen DNS-Änderungen erforderlich voraussetzen oder durchführen.
- Postfächer und Maildaten nicht in eine Website-Dateisynchronisierung aufnehmen. Vorher und nachher empfangen und senden lassen; E-Mail-Testnachrichten nur mit ausdrücklichem Auftrag versenden.

## 4. Testbereitstellung nach Freigabe

- Getrennte Dokumentwurzel mit Zugriffsschutz und HTTPS verwenden; kein Unterordner, der wegen der absoluten CSS-/Bildpfade die Produktionsdateien lädt. Bestehende Root-Dateien bleiben erhalten.
- Nur referenzierte Website-Dateien ausliefern: `index.html`, `impressum.html`, `datenschutz.html`, `cookie-hinweise.html`, `style.css`, `favicon.ico`, `assets/gaby-entspannt.webp`. Vollständige Referenzprüfung unmittelbar davor wiederholen. Originalbilder bleiben lokal/Git erhalten.
- Keine `.git`, `.openai`, README, TODO, Prüfberichte oder unreferenzierten großen Bildvarianten auf das Ziel übertragen. Freigabe verhindert nicht die Notwendigkeit fertiggestellter rechtlicher Seiten.
- Smartphone/Desktop, echte iOS-/Android-Geräte, Tastatur, alle Preislisten, Bild, Metadaten und Links prüfen. HTTP-Header auf Cookies, Browser auf Speicherzugriffe und Server auf Protokollierung prüfen. Cookie-Namen/Werte mit Zugangs- oder Sitzungstokens nicht in Git dokumentieren.
- Weiterleitungszuordnung aus `WEITERLEITUNGEN.md` auf dem Testserver umsetzen und prüfen. `/hvl.html` zuvor entscheiden.

## 5. Umschaltung nach ausdrücklicher Freigabe

- Getesteten lokalen Commit und Dateiprüfsummen festhalten. Keine zusätzliche Sicherung gemäß Nutzerentscheidung voraussetzen.
- Neue Dateien in einem getrennten Verzeichnis vorbereiten; je nach Paket die Domain-Dokumentwurzel kontrolliert umstellen oder einen vom Anbieter unterstützten atomaren Austausch nutzen. Keine pauschale Synchronisierung mit Löschoption.
- Vorhandene Serverregeln behutsam ergänzen; Weiterleitungen erst aktivieren, wenn Ziele erreichbar sind. Dokumentierte E-Mail-/DNS-Konfiguration erhalten.
- Hauptseite, alle rechtlichen Seiten, Preislisten, Bild, HTTPS und jede Alt-URL nach dem Wechsel prüfen. Mail-Senden/-Empfangen gesondert prüfen lassen.

## 6. Rückfall

- Rückfall auslösen bei fehlenden Seiten/Bildern, Weiterleitungsschleifen, SSL-Fehlern, nicht nutzbarem Kontakt oder E-Mail-Störung. Ergebnis und Zeitpunkt festhalten.
- Falls die vorherige Dokumentwurzel beim getrennten Bereitstellen erhalten geblieben ist, diese wieder zuordnen. Weitere Wiederherstellung nur aus tatsächlich vorhandenen Beständen; keine neu erstellte Sicherung voraussetzen. Maildaten und DNS-Konfiguration erhalten.
- Alte Haupt-/Unterseiten, HTTPS und E-Mail erneut prüfen lassen. Neue Dateien für Ursachenanalyse erhalten; keinen ungezielten rekursiven Löschbefehl ausführen.

## Offizielle Hinweise für die Paketprüfung

- [Host Europe: Logdateien und konfigurierbare IP-Anonymisierung](https://www.hosteurope.de/faq/webhosting/webhosting-logfiles/logfiles-einsehen-und-aendern)
- [Host Europe: Backup für WebHosting](https://www.hosteurope.de/faq/webhosting/restore-und-backup)
- [Host Europe: Vertrag zur Auftragsverarbeitung](https://www.hosteurope.de/faq/vertrag-und-rechnungen/vertrag/adv-vertrag)

Diese Dokumentation bestätigt keine konkrete Log-Aufbewahrungsdauer, keinen abgeschlossenen AVV und keinen tatsächlichen Serverstandort des gebuchten Pakets.

[Host Europe: SFTP und FTPES](https://www.hosteurope.de/faq/webhosting/hochladen-von-webinhalten-ftp/ftp-verschluesselt-uebertragen): SFTP verwendet den SSH-Zugang; FTPES ist die TLS-verschlüsselte FTP-Variante. Die richtige Verbindung für dieses Paket muss anhand des Kundenportals geprüft werden.

## Veröffentlichung am 11.10.2026

Auf ausdrücklichen Nutzerauftrag wurden die sieben referenzierten Dateien aus Commit f1e9c33 auf den bisherigen Host-Europe-Webspace übertragen. Die vorhandene FileZilla-Verbindung wurde per FTPES mit Zertifikatsprüfung verwendet; keine Zugangsdaten in Projekt, Git oder zusätzlichen Dateien gespeichert. Beide Domainvarianten wurden vorab durch eine temporäre Testdatei der FTP-Dokumentwurzel zugeordnet; die Testdatei wurde entfernt. Der FTP-Zugang ist auf die Dokumentwurzel eingeschränkt, daher ist /www nicht als Unterverzeichnis erreichbar.

Alle sieben veröffentlichten Dateien: HTTP 200, SHA-256 identisch zum lokalen Stand, kein Set-Cookie-Header beobachtet. Startseite im Browser bei 1280 und 390 Pixeln ohne horizontalen Überlauf; Foto geladen, Favicon verlinkt, Herrenpreisliste erfolgreich geöffnet. DNS und E-Mail-Konfiguration wurden nicht geändert; keine E-Mail-Testnachricht versandt. Zusätzliche Sicherung entfiel gemäß Nutzerentscheidung. Rechtliche Seiten bleiben sichtbar gekennzeichnete Entwürfe. Alte URL-Weiterleitungen, tatsächliche Hosting-/Datenschutzdetails und echte Geräteprüfungen bleiben offen.
