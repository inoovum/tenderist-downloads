# tenderist-downloads

Öffentliche Download-Ablage für **TENDERIST POS**.

Die stationären Desktop-Kassen (Windows und macOS) beziehen ihre Updates
automatisch über die **GitHub Releases** dieses Repos: Die App prüft beim
Start `releases/latest` und bietet ein In-App-Update an. Manuelle Downloads
gibt es über die Release-Assets bzw. die unten verlinkten Dateien.

## Aktuelle Version herunterladen

Immer den neuesten Build gibt es über das jeweils **letzte Release**:

- **Windows (x64):**
  <https://github.com/inoovum/tenderist-downloads/releases/latest/download/tenderist-pos-windows-x64.zip>
- **macOS (Apple Silicon & Intel, Universal):**
  <https://github.com/inoovum/tenderist-downloads/releases/latest/download/tenderist-pos-macos.dmg>

Alle Versionen: <https://github.com/inoovum/tenderist-downloads/releases>

## Installation

### Windows

1. ZIP herunterladen und entpacken.
2. Den gesamten Ordnerinhalt an den gewünschten Installationsort kopieren.
3. `tenderist_pos.exe` starten.

Updates installiert die App unter Windows selbst (Download, Austausch,
Neustart).

### macOS

1. DMG herunterladen und öffnen.
2. `tenderist_pos.app` auf den **Programme**-Alias ziehen.
3. Beim ersten Start meldet macOS ggf. „nicht verifizierter Entwickler"
   (die App ist ad-hoc signiert, nicht notarisiert). In dem Fall die App
   einmalig per **Rechtsklick → Öffnen** starten.

Ein Update lädt die App als DMG herunter und öffnet es; danach die neue
`tenderist_pos.app` erneut nach **Programme** ziehen und neu starten.

## Release-Konvention

- Tag: `v<version>` (z. B. `v1.6.13`)
- Windows-Asset: `tenderist-pos-windows-x64.zip`
- macOS-Asset: `tenderist-pos-macos.dmg`

Die Builds werden über die GitHub-Workflows `pos-windows-release.yml` und
`pos-macos-release.yml` im App-Repo erzeugt und hierher veröffentlicht.
