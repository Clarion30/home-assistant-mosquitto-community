# Mosquitto Community Broker für Home Assistant

Dieses Repository stellt eine inoffizielle Home-Assistant-App bereit, die den offiziellen Eclipse-Mosquitto-Broker verwendet.

## Was macht die App?

Die App startet einen lokalen MQTT-Broker direkt auf dem Home-Assistant-System. Geräte und Dienste wie ESPHome können sich damit per MQTT mit Home Assistant verbinden.

### Funktionen

- Eclipse Mosquitto 2.1.2
- MQTT auf Port 1883
- Benutzername- und Passwortschutz
- keine anonymen MQTT-Verbindungen
- persistente MQTT-Daten
- Debugprotokollierung bei Bedarf ein- und ausschaltbar
- geeignet für Home Assistant und ESPHome
- automatischer Start mit Home Assistant
- automatische Prüfung auf neue offizielle Eclipse-Mosquitto-Versionen über GitHub Actions

## Warum gibt es diese App?

Sie wurde erstellt, weil beim regulären Home-Assistant-Mosquitto-Add-on in einer konkreten Konfiguration ein reproduzierbares MQTT-Problem mit ESPHome und QoS 2 auftrat. Diese App verwendet deshalb direkt das offizielle Eclipse-Mosquitto-Docker-Image.

## Installation

In Home Assistant unter **Einstellungen → Apps → App-Store → Repositories** dieses Repository hinzufügen:

`https://github.com/Clarion30/home-assistant-mosquitto-official`

Anschließend **Mosquitto Community Broker** installieren, Benutzername und Passwort setzen und die App starten.

> Wichtig: Das reguläre Mosquitto-Broker-Add-on darf nicht gleichzeitig laufen, da beide Port 1883 verwenden.

## Unterstützte Plattformen

- `amd64` – unterstützt
- `aarch64` – freigegeben, aber vom Autor bisher nicht auf echter ARM64-Hardware getestet. Aufgrund des offiziellen Multi-Arch-Eclipse-Mosquitto-Images und der einfachen Shell-Startlogik sollte die App funktionieren.

Wenn du `aarch64` verwendest und Probleme feststellst, bitte ein GitHub-Issue mit den Home-Assistant- und App-Logs eröffnen.

## Datenschutz

Die App enthält aktuell keine Telemetrie und übermittelt keine Installations- oder Nutzungsdaten an den Autor.

## Hinweis

Dies ist eine inoffizielle Community-App. Sie ist nicht mit der Eclipse Foundation, dem Eclipse-Mosquitto-Projekt oder Home Assistant verbunden und wird von diesen nicht offiziell unterstützt oder empfohlen.

Mosquitto und Eclipse Mosquitto sind Bezeichnungen des jeweiligen Eclipse-Projekts. Die App verwendet das öffentlich bereitgestellte Docker-Image `eclipse-mosquitto`.
