# Repo-Einrichtung für das Unreal-Projekt DarkVigil

Diese beiden Dateien kommen **in den Unreal-Projektordner**, direkt neben `DarkVigil.uproject`:

| Datei | Wozu |
|---|---|
| `.gitignore` | Sagt Git, was **nicht** hochgeladen wird: Caches, Kompilier-Reste und die Assets aus dem Game Animation Sample / Fab |
| `.gitattributes` | Sagt Git, welche großen Dateien über **Git LFS** gespeichert werden (`.uasset`, `.umap`, Texturen, Audio …) |

## Schritte

1. Unreal-Projekt erstellen und **einmal öffnen** (damit alle Ordner existieren). Dann Unreal schließen.
2. Beide Dateien aus diesem Ordner nach `C:\DarkVigilProjekt\DarkVigil\` kopieren.
3. Im Projektordner einen Ordner `Docs` anlegen und `KONZEPT.md` + `PROJECT_PROGRESS.md` hineinkopieren.
4. In `Content` einen leeren Ordner `DarkVigil` anlegen – hier kommt später unser eigener Content hinein.
5. GitHub Desktop → **File → Add local repository** → `C:\DarkVigilProjekt\DarkVigil` auswählen.
   GitHub Desktop sagt dann, dass dort noch kein Repository ist → **create a repository** anklicken
   (bei „Git ignore" und „License" **None** lassen – unsere `.gitignore` liegt ja schon da).
6. Falls GitHub Desktop fragt, ob **Git LFS** eingerichtet werden soll → **Ja / Initialize Git LFS**.
7. **Bevor du committest:** Im Reiter „Changes" links prüfen, was hochgeladen würde.
   Es sollten nur ein paar Dateien sein (`DarkVigil.uproject`, `Config/...`, `Docs/...`, die beiden Git-Dateien).
   **Wenn dort tausende Dateien oder Ordner wie `Content/Characters` auftauchen → stopp und Screenshot an Claude.**
8. Commit-Nachricht: `Initial project setup` → **Commit to main**.
9. **Publish repository** → Name `DarkVigil` → Häkchen bei **Keep this code private** → Publish.
