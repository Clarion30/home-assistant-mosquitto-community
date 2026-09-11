# Mosquitto Official – Dokumentation

## Verwendung

Die App stellt einen MQTT-Broker auf Port 1883 der Home-Assistant-IP bereit.

## Konfiguration

### username

MQTT-Benutzername. Es ist bewusst kein Standardwert vorgegeben. Bitte einen eigenen Benutzernamen eintragen.

### password

Passwort für den MQTT-Benutzer. Das Passwort muss gesetzt sein.

### debug

Schaltet die ausführliche Mosquitto-Protokollierung ein oder aus.

Bei `false` werden normale Informations-, Warn- und Fehlermeldungen angezeigt.

Bei `true` verwendet Mosquitto `log_type all`.

## Unterstützte Plattformen

- `amd64` – unterstützt
- `aarch64` – freigegeben, aber bisher nicht auf echter ARM64-Hardware getestet. Aufgrund des offiziellen Multi-Arch-Eclipse-Mosquitto-Images und der einfachen Shell-Startlogik sollte die App funktionieren.

## Wichtiger Hinweis

Das reguläre Home-Assistant-Mosquitto-Add-on darf nicht gleichzeitig laufen. Beide MQTT-Broker würden Port 1883 der Home-Assistant-IP verwenden.

## Diagnose

Für eine ausführliche Fehlersuche kann vorübergehend `debug: true` gesetzt werden. Nach der Diagnose sollte Debug wieder ausgeschaltet werden.

## Haftungs- und Projekthinweis

Diese App ist ein unabhängiges Community-Projekt und keine offizielle
App der Eclipse Foundation, des Eclipse-Mosquitto-Projekts oder von
Home Assistant.

Die Verwendung erfolgt auf eigene Verantwortung. Vor Aktualisierungen
sollte eine Sicherung der App-Konfiguration vorhanden sein.
