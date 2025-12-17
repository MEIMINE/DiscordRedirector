# Discord Redirector

Ein einfacher Discord Server Redirector mit schönen Embeds.

## Einrichtung

1. **Discord Invite Link anpassen**
   - Ersetze `DEININVITELINK` in `index.html` mit deinem Discord Invite Code

2. **Server Informationen anpassen**
   - Titel: Ändere "HIER DEIN DISCORD SERVER NAME" und "Discord Server Titel"
   - Beschreibung: Ändere "Discord Server Beschreibung"
   - Tags: Füge relevante Tags hinzu
   - Embed Link: Trage deine finale URL ein

3. **Bilder hinzufügen**
   - Platziere dein Server-Bild als `image.png` im Root-Verzeichnis
   - Favicon: Platziere dein Icon in `assets/favicon.ico`

## Deployment auf Vercel

### Mit Vercel CLI
```bash
npm i -g vercel
vercel login
vercel
```

### Mit GitHub
1. Push dein Repository zu GitHub
2. Gehe zu [vercel.com](https://vercel.com)
3. Importiere dein GitHub Repository
4. Vercel deployed automatisch

## Benötigte Dateien

- `index.html` - Hauptdatei
- `image.png` - Dein Server-Bild für das Embed (1920x1080 empfohlen)
- `assets/favicon.ico` - Dein Server-Icon (optional)
- `vercel.json` - Vercel Konfiguration (bereits vorhanden)

## Anpassungen

Die Weiterleitung erfolgt nach 1 Sekunde. Um die Verzögerung zu ändern, passe in `index.html` an:
```html
<meta http-equiv="refresh" content="1; url=...">
```
Ändere die `1` auf die gewünschte Anzahl Sekunden.
