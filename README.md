# Jellyfin MP3 Downloader

> Web-Anwendung zum Herunterladen von Audioinhalten aus YouTube/YouTube-Music
> als MP3, mit editierbaren Metadaten und direkter Ablage in einem bestehenden
> Musikbestand (z. B. für Jellyfin).

<!-- Optional: Badges hier einfügen, z. B. Build-Status, Lizenz, Docker Pulls -->

## Inhaltsverzeichnis

- [Über das Projekt](#über-das-projekt)
- [Funktionen](#funktionen)
- [Architektur](#architektur)
- [Voraussetzungen](#voraussetzungen)
- [Installation & Start](#installation--start)
- [Konfiguration](#konfiguration)
- [Entwicklung](#entwicklung)
- [Roadmap](#roadmap)
- [Bekannte Einschränkungen](#bekannte-einschränkungen)

## Über das Projekt

Kurzbeschreibung, warum das Projekt existiert und welches Problem es löst.
(z. B.: manuelles Herunterladen und Taggen von Songs für die eigene
Musikbibliothek war umständlich; dieses Tool automatisiert Download,
Metadaten-Pflege und Einsortierung in eine bestehende, Jellyfin-kompatible
Ordnerstruktur.)

## Funktionen

- [ ] Einzel-Song-Download über YouTube-/YouTube-Music-Link
- [ ] Automatisches Laden von Titel und Interpret als Vorschlag
- [ ] Manuelle Bearbeitung von Titel, Interpret, Dateiname vor dem Download
- [ ] Playlist-Download (mehrere Songs komfortabel erfassen, keine
      Playlist-Struktur im Zielbestand)
- [ ] Duplikat-Prüfung gegen bestehenden Musikbestand (dateibasiert, keine DB)
- [ ] Konfigurierbarer Zielpfad (Betreiber-Konfiguration, nicht im laufenden
      Betrieb änderbar)

## Architektur

Kurzer Überblick über die grundlegende Aufteilung des Projekts (Schichten,
Verantwortlichkeiten), ohne Implementierungsdetails.

<!-- Ausführliche Architektur-Dokumentation folgt ggf. später unter docs/,
     sobald die Struktur final steht. -->

## Voraussetzungen

- Docker & Docker Compose
- Zugriff auf ein Zielverzeichnis für den Musikbestand (lokal oder Netzwerkfreigabe)

## Installation & Start

<!-- Schritt-für-Schritt-Anleitung, sobald der Code steht:
     Repo klonen → Konfigurationsdatei anlegen → Container starten -->

## Konfiguration

Beschreibung, welche Einstellungen es gibt (z. B. Pfad zum Musikbestand) und
wo diese vorgenommen werden (Konfigurationsdatei, nicht über die Weboberfläche).

## Entwicklung

Hinweise für lokale Entwicklung (z. B. abweichende Konfiguration für
Testzwecke, Ausführen der Tests).

## Roadmap

- [ ] MVP: Einzel-Song-Download
- [ ] Playlist-Download
- [ ] ggf. spätere Erweiterungen (bewusst offen halten, nicht vorwegnehmen)

## Bekannte Einschränkungen

- Abhängigkeit von Drittanbieter-Bibliothek zur Inhaltsextraktion; Verhalten
  kann sich durch Änderungen der Zielplattform ändern
- Keine Mehrbenutzer-/Rechteverwaltung vorgesehen (Einzelnutzer-Tool)
