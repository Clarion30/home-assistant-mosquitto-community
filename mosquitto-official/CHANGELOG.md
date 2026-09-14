# Änderungsprotokoll

## 1.1.7

- Repository von `home-assistant-mosquitto-official` auf `home-assistant-mosquitto-community` umbenannt
- Repository-Links in App-Konfiguration und Dokumentation aktualisiert

## 1.1.6

- Unterstützung für `aarch64` in Home Assistant freigegeben
- Hinweis ergänzt, dass ARM64 bisher nicht auf echter Hardware getestet wurde, aber aufgrund des offiziellen Multi-Arch-Eclipse-Mosquitto-Images funktionieren sollte

## 1.1.5

- Standardwert `mqtt` für den MQTT-Benutzernamen entfernt
- Benutzername muss jetzt bewusst selbst eingetragen werden

## 1.1.4

- Projektlink auf das eigene GitHub-Repository geändert

## 1.1.3

- Überschrift der Dokumentation auf `Mosquitto Community Broker` geändert
- Darstellung der App vereinheitlicht

## 1.1.2

- Sichtbaren Namen in `Mosquitto Community Broker` geändert
- Kennzeichnung als inoffizielle Community-App ergänzt
- Beschreibung und Dokumentation überarbeitet

## 1.1.1

- Lokale App-Struktur bereinigt
- Alte Sicherung mit doppelter config.yaml entfernt
- Update-Erkennung über Home Assistant korrigiert
- Dokumentation und Änderungsprotokoll ergänzt

## 1.1.0

- Internen Slug von `mosquitto_official_test` auf `mosquitto_official` geändert
- Ein- und ausschaltbare Debugprotokollierung hinzugefügt
- Lesbares Zeitstempelformat ergänzt
- Dokumentation ergänzt
- Änderungsprotokoll ergänzt
- Beschreibung der App erweitert

## 1.0.3

- Zeitstempelformat mit Datum und Uhrzeit ergänzt
- Eclipse Mosquitto 2.1.2 verwendet
- MQTT-QoS-2-Kommunikation mit ESPHome erfolgreich getestet

## 1.0.2

- Benutzername und Passwort aus `/data/options.json` übernommen
- Passwortdatei automatisch erzeugt
- Persistente Mosquitto-Daten aktiviert

## 1.0.1

- Erste funktionsfähige lokale Version
- Port 1883 über das Hostnetz bereitgestellt
