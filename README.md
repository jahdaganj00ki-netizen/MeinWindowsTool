# Hallo aus der Cloud!

Ein einfaches .NET 8 Konsolenprogramm, das in einer Linux-basierten Cloud-Sandbox kompiliert wird und auf Windows 10 (64-Bit) läuft.

## Anleitung

### 1. Programm kompilieren

Führe diesen Befehl im Cloud-Terminal aus, um eine lauffähige Windows-Exe zu erstellen:

```bash
dotnet publish -c Release -r win-x64 --self-contained true -p:PublishSingleFile=true
```

### 2. Exe finden

Die kompilierte Datei findest du hier:

```
bin/Release/net8.0/win-x64/publish/MeinWindowsTool.exe
```

### 3. Exe herunterladen und ausführen

1. Lade die `MeinWindowsTool.exe` von der Cloud auf deinen Windows 10 Laptop herunter
2. Führe die Datei aus
3. Du solltest die Nachricht "Hallo aus der Cloud!" sehen

## Technische Details

- **Sprache**: C# mit .NET 8
- **Plattform**: Windows 10 (64-Bit)
- **Cross-Compilation**: Wird in einer Linux-basierten Cloud-Sandbox kompiliert
- **UI**: Einfache Konsolenanwendung

## Support

Falls du Fragen hast, kontaktiere den Entwickler.