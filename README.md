# Computercraft Lua Script README

## Beschreibung
Dieses Repository enthält Lua-Skripte für die Verwendung mit Computercraft, einer Mod für das Spiel Minecraft. Diese Skripte automatisieren bestimmte Aufgaben und verbessern die Funktionalität von Computercraft-Computerprogrammen.

## Voraussetzungen
- Minecraft mit Computercraft-Mod installiert
- Computercraft-Computer oder -Turtles im Spiel

## Skripte herunterladen

### Über Pastebin
1. Öffne das Computercraft-Computerprogramm oder die Turtle im Spiel.
2. Führe den folgenden Befehl aus, um das Skript von Pastebin herunterzuladen:

   ```lua
   pastebin get PASTE_CODE FILE_NAME
   ```

   Ersetze `PASTE_CODE` durch den Pastebin-Code des Skripts und `FILE_NAME` durch den gewünschten Dateinamen.

### Über HTTP (mit wget-ähnlichem Befehl)
1.	Öffne das Computercraft-Computerprogramm oder die Turtle im Spiel.
2.	Führe den folgenden Befehl aus, um das Skript von einem HTTP-Server herunterzuladen:

   ```lua
   shell.run(„wget SCRIPT_URL FILE_NAME“)
   ```

2.	Ersetze SCRIPT_URL durch die URL des Skripts und FILE_NAME durch den gewünschten Dateinamen.

### Über HTTP (mit `http`-API)
1. Öffne das Computercraft-Computerprogramm oder die Turtle im Spiel.
2. Führe den folgenden Befehl aus, um das Skript von einem HTTP-Server herunterzuladen:

   ```lua
   local url = „SCRIPT_URL“
   local response = http.get(url)
   
   if response then
     local content = response.readAll()
     response.close()
     
     local file = fs.open(„FILE_NAME“, „w“)
     file.write(content)
     file.close()
   else
     print(„Fehler beim Herunterladen des Skripts.“)
   end
   ```

   Ersetze `SCRIPT_URL` durch die URL des Skripts und `FILE_NAME` durch den gewünschten Dateinamen.

## Verwendung
1. Lade die Lua-Skripte herunter oder klonen Sie dieses Repository.
2. Kopiere die Skripte auf den Computer oder die Turtle im Spiel.
3. Starte das gewünschte Computercraft-Programm auf dem Computer oder der Turtle.

## Beispiele
- **autoFarm.lua**: Automatisiert den Ernteprozess für landwirtschaftliche Betriebe.
  
```lua
— Beispielcode oder Anleitung hier einfügen
```

- **miningTurtle.lua**: Programm für eine Turtle, um automatisch Ressourcen abzubauen.

```lua
— Beispielcode oder Anleitung hier einfügen
```

## Beitrag
Fühlen Sie sich frei, Fehler zu melden, Verbesserungen vorzuschlagen oder neue Skripte beizutragen. Öffnen Sie einfach ein Issue oder eine Pull-Anfrage.

## Lizenz
Dieses Projekt ist unter der [MIT-Lizenz](LICENSE) lizenziert - weitere Informationen finden Sie in der Datei LICENSE.

Viel Spaß beim Automatisieren in Minecraft mit Computercraft!