# PROJECT_PROGRESS – Dark Vigil

> Diese Datei liest Claude zu Beginn jeder Sitzung. Hier steht immer, wo wir gerade stehen.
> Hinweis: Sobald das eigene Repo **DarkVigil** (UE5-Projekt) existiert, ziehen diese Dateien dorthin um.

## Aktueller Stand (2026-11-09)

**Phase:** 0 – Vorbereitung (noch kein Unreal-Projekt)

### Erledigt
- [x] Anforderungen besprochen
- [x] Entscheidung Engine: **Unreal Engine 5** (C++ + Blueprints)
- [x] Entscheidung Sprache: **Englische Sprachausgabe**, Untertitel/Menüs **Deutsch + Englisch**, Code auf Englisch, Projektdokumente auf Deutsch
- [x] Visual Studio 2026 Community: Installation gestartet (Workloads: Desktopentwicklung mit C++, Spieleentwicklung mit C++, Unreal Engine Test Adapter; Komponente MSVC v143 14.38)
- [x] Konzept v1.0 geschrieben und von Dennis freigegeben → `KONZEPT.md`

### Läuft gerade (Dennis)
- [ ] Epic Games Launcher + Unreal Engine 5 installieren
- [ ] Game Animation Sample von Fab holen

### Offen / nächste Schritte
1. ~~Feedback zum Konzept~~ → **Konzept v1.0 freigegeben** ✅
2. **Dennis:** UE-Version mitteilen, Projekt `DarkVigil` aus dem Game Animation Sample erstellen, in C++-Projekt umwandeln
3. **Gemeinsam:** Neues GitHub-Repo `DarkVigil` mit Git LFS + `.gitignore` / `.gitattributes` für Unreal
4. **Claude:** Technischer Entwicklungsplan (`TECH_PLAN.md`), `ASSET_LIST.md`, Grafikprofile Niedrig/Mittel/Hoch/Episch
5. **Claude:** C++-Grundgerüst Phase 1 (Kamera, Targeting, Freeflow-Kern, Konter, Ausweichen, 1 Gegnertyp, Stealth-Takedown)

### Nächster konkreter Schritt
Warten auf Dennis: UE5-Installation fertig + UE-Version mitteilen.

## Wichtige Hinweise für Claude
- In der Cloud-Sitzung gibt es **kein Unreal** → C++ kann dort nicht kompiliert werden. Nach jedem größeren C++-System auf Kompilier-Test durch Dennis warten und in dieser Datei vermerken.
- In kleinen Schritten arbeiten, nach jedem Schritt committen und pushen.
