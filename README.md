Disclaimer: This was made modstly with the help of AI, so I don't take too much credit for it. It was a decent amount of work to get right and help with but I don't want to take too much credit for this.
# Desktop-Virtual-Pinball
VPIN for landscape monitors
# VPinball Launcher

A dark arcade-style frontend for Visual Pinball X tables.

## Setup

**Tables:** Map to your directory with your VPX files (📁 SCAN FOLDER button auto-imports everything)

**Executable:** Select your vpinball exe — default is `C:\RetroBat\emulators\vpinball\vpinballx64.exe`

**Artwork:** Optional folder path for wheel images (circular table art, fuzzy-matched by name)

**PINemHi:** Navigate to the main PINemHi directory. It needs the `[romfind]` section for ROM name matching (a blank example is in the PINemHi Example folder if yours doesn't have it). The launcher uses that to look up ROM names, then reads scores from `PINemHi LeaderBoard\TOP10_Personal\`. Matching isn't perfect — if a table shows the wrong scores, open Edit Table and manually set the ROM name override.

## Controls

| Key | Action |
|-----|--------|
| Left Shift | Previous table |
| Right Shift | Next table |
| Z | Page back |
| / | Page forward |
| Enter | Launch selected table |
| Ctrl + Click | Multi-select tables |

## Features

- 🎯 Wheel image display with fuzzy filename matching
- 🏆 PINemHi personal high scores in the detail panel
- ⭐ Favorites, play count tracking, recently played
- 🔍 VPS database lookup for manufacturer/year/ROM info
- 📁 Folder sync — scan adds new tables, removes deleted ones
- 🎮 Multi-select with bulk move to category or bulk remove
- 🏅 Scores-to-beat strip at the top (6 manual entries)
- 🔤 Adjustable font size in Settings

## Data Location

All your library data, settings, play history, and high score entries are stored at:

```
C:\Users\[YourName]\AppData\Roaming\vpinball-launcher\tables.json
```

Back this file up to keep your full setup. Copy it to another machine to transfer everything.

## Building

```bash
npm install
npm start        # run in development
npm run build    # build Windows installer to dist/
```
