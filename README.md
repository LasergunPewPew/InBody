# InBody Verlauf

Kleine Web-App, um InBody-Messungen zu sammeln und zu vergleichen – direkt im Handy-Browser.

## Funktionen

- **InBody-PDF einlesen** (Ergebnisbogen InBody 970S): Die Werte werden direkt im Browser erkannt, ohne Upload und ohne Konto. Jedes Feld zeigt den passenden Ausschnitt aus der PDF zum Prüfen.
- **CSV-Export der InBody-App** importieren (bereits vorhandene Messungen werden erkannt).
- **Werte von Hand** eintragen.
- **Übersicht** mit Veränderungen zur vorherigen Messung, **Vergleich** zweier Messungen, **Verlaufskurven** für jeden Wert.
- **Mehrere Personen** über die Auswahl oben.
- **Sicherung** herunterladen und wieder laden.

## Datenschutz

Alle Messwerte bleiben im Browser des jeweiligen Geräts (localStorage). Es werden keine Daten an einen Server geschickt. Nachgeladen werden nur zwei Bibliotheken von cdnjs (Chart.js für die Kurven und pdf.js zum Öffnen der PDF).

Wichtig: Wer die Browserdaten löscht, löscht auch die Messungen – daher ab und zu „Sicherung herunterladen“ nutzen.

## Einrichten mit GitHub Pages

1. Alle Dateien dieses Ordners in ein öffentliches Repository hochladen.
2. **Settings → Pages → Branch: `main` / Ordner `/ (root)`** wählen und speichern.
3. Nach ca. einer Minute ist die App unter `https://<benutzername>.github.io/<repository>/` erreichbar.
4. Auf dem iPhone in Safari öffnen → Teilen → **Zum Home-Bildschirm**.

## Hinweise

- Die PDF-Erkennung ist auf das Layout des InBody-970S-Bogens abgestimmt. Bei anderen Geräten zeigt die App eine Warnung; die Werte können dann von Hand eingetragen werden.
- Die viszerale Fettfläche steht auf dem Bogen nur in einer Grafik und wird daher von Hand eingetragen (die App zeigt den Ausschnitt an).
