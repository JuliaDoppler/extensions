This extension contains useful extensions for working with Angular.

# Erstellen einer Extension für VS Code als Extension Pack
Folgende Files muss eine Extension zumindest enthalten:
- `CHANGELOG.md`
- `LICENSE.md`
- `package.json`
  - Informationen zum Aufbau des `package.json`: https://code.visualstudio.com/api/references/extension-manifest
- `README.md`
- VSIX-Datei
  - Die VSIX-Datei wird verwendet, um die Extension im Marketplace zu publishen.
  - Diese Datei dient eigentlich an Archiv und beinhaltet alle anderen Files aus dem Ordner, wo die Datei `package.json` liegt.

optional
- Ein Bild, dass als 

## Erstellung einer VSIX Datei
- Öffnen der Powershell als Admin
- Ausführen des Kommandos `Set-ExecutionPolicy RemoteSigned -Scope CurrentUser`
- Installierung von vsce ist notwendig `npm install -g vsce`
- Navigieren in den Ordner, wo die Datei `package.json` liegt.
- Aufruf des Kommandos `vsce package`. Gibt es keine Kompelierfehler, wird eine vsix-Datei erstellt.
-  Diese Datei kann dann über den MarketPlace von Visual Studio Code hochgeladen werden. (Pusblishen ist in wenigen Minuten durch. Danach kann die Extension gleich verwendet werden.

Mehr Informationen sind unter https://code.visualstudio.com/api/working-with-extensions/publishing-extension ersichtlich.
