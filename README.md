# Video → Live Foto

Wandelt Videos in ein Live-Foto-Paar (JPG + MOV) um. Läuft komplett im Browser, ffmpeg.wasm liegt in `vendor/`.
Die große `ffmpeg-core.wasm` ist in 3 Teile (je ca. 11 MB) zerlegt, damit der GitHub-Upload im Browser (max. 25 MB pro Datei) klappt. Die Seite setzt sie beim Laden wieder zusammen. Alle Teile müssen hochgeladen werden.

## Auf GitHub Pages veröffentlichen
1. Neues Repo anlegen, alle Dateien dieses Ordners hochladen (inkl. `vendor/` und `.nojekyll`).
2. Settings → Pages → Deploy from a branch → `main` → `/ (root)`.
3. Erreichbar unter `https://DEIN-NAME.github.io/REPO-NAME/`.

## Lokal testen
`python3 -m http.server` im Ordner, dann http://localhost:8000 öffnen.
