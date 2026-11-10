# PROJECT_PROGRESS – Dark Vigil

> Diese Datei liest Claude zu Beginn jeder Sitzung. Hier steht immer, wo wir gerade stehen.
> Hinweis: Sobald das eigene Repo **DarkVigil** (UE5-Projekt) existiert, ziehen diese Dateien dorthin um.

## Aktueller Stand (2026-11-10)

**Phase:** 0 – Vorbereitung (Engine installiert, Unreal-Projekt wird gerade angelegt)

### Erledigt
- [x] Anforderungen besprochen
- [x] Entscheidung Engine: **Unreal Engine 5.8** (C++ + Blueprints) – letzte große UE5-Version, Game Animation Sample ist für 5.8 aktualisiert
- [x] Entscheidung Sprache: **Englische Sprachausgabe**, Untertitel/Menüs **Deutsch + Englisch**, Code auf Englisch, Projektdokumente auf Deutsch
- [x] Visual Studio 2026 Community (18.11.3) installiert – Workloads: Desktopentwicklung mit C++, Spieleentwicklung mit C++, Unreal Engine Test Adapter; zusätzliche Komponenten: MSVC v143 **14.38** und **14.44**
- [x] Konzept v1.0 geschrieben und von Dennis freigegeben → `KONZEPT.md`
- [x] Epic Games Launcher + **Unreal Engine 5.8.4** installiert
- [x] Game Animation Sample in der Fab-Bibliothek

### Läuft gerade (Dennis)
- [ ] Projekt **`DarkVigil`** aus dem Game Animation Sample erstellen (Speicherort `C:\DarkVigilProjekt`, Projekt liegt dann in `C:\DarkVigilProjekt\DarkVigil`)
- [ ] Projekt öffnen und mit **Play** testen (herumlaufen)

### Offen / nächste Schritte
1. **Dennis:** Projekt in ein C++-Projekt umwandeln (Tools → New C++ Class) = erster Kompilier-Test mit VS 2026
2. **Gemeinsam:** Git für Windows + Git LFS installieren, neues **privates** GitHub-Repo `DarkVigil`, erster Push
3. **Claude:** Projekt analysieren, dann technischer Entwicklungsplan (`TECH_PLAN.md`), `ASSET_LIST.md`, Grafikprofile Niedrig/Mittel/Hoch/Episch
4. **Claude:** C++-Grundgerüst Phase 1 (Kamera, Targeting, Freeflow-Kern, Konter, Ausweichen, 1 Gegnertyp, Stealth-Takedown)

### Nächster konkreter Schritt
Warten auf Dennis: Projekt `DarkVigil` erstellt und Play funktioniert. Danach Schritt 1 (C++-Umwandlung).

## Wichtige Hinweise für Claude
- **Toolchain UE 5.8:** Epic empfiehlt MSVC **14.44** (VS-2022-Toolset) oder **14.50** (VS-2026-Toolset). Mit VS 2026 gibt es bekannte Compile-Fehler (`<hash_map>`); im Zweifel das 14.44-Toolset nutzen. Exakte Werte stehen in `Engine/Config/Windows/Windows_SDK.json`.
- **Vorschlag Repo-Aufbau (noch mit Dennis abstimmen):** Ins Git-Repo kommen nur `Source/`, `Config/`, `DarkVigil.uproject`, die Dokumente und **eigener** Content unter `Content/DarkVigil/` (über Git LFS). Die Inhalte des Game Animation Sample und Fab-Assets bleiben außerhalb von Git (Größe, langsames Internet, Epic-Lizenz) und werden in `ASSET_LIST.md` dokumentiert. Regel dazu: Sample-Assets nicht direkt verändern, sondern Kind-Blueprints oder Kopien unter `Content/DarkVigil/` anlegen.
- In der Cloud-Sitzung gibt es **kein Unreal** → C++ kann dort nicht kompiliert werden. Nach jedem größeren C++-System auf Kompilier-Test durch Dennis warten und in dieser Datei vermerken.
- In kleinen Schritten arbeiten, nach jedem Schritt committen und pushen.
