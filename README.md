# Delete Nearest Marker to Cursor

**English** · [Русский](README_RU.md)


Deletes the marker closest to the edit cursor by absolute distance. Regions are ignored — markers only.

## Installation

### ReaPack

Import the [Patch34 ReaPack catalog](https://raw.githubusercontent.com/patch-34/patch34-reapack/main/index.xml) via **Extensions → ReaPack → Import repositories…** and install **Delete Nearest Marker to Cursor** from **Browse packages**.

### Manual installation

1. In REAPER: **Actions → Show action list…**
2. Click **ReaScript: Load…**
3. Select `Delete_Nearest_Marker_To_Cursor.lua`
4. Optionally assign a keyboard shortcut

## How it works

The script scans all project markers, calculates `abs(marker_pos - cursor_pos)` for each one, and deletes the nearest. The action is fully undoable.

## Notes

- Regions are skipped entirely
- If the project has no markers (only regions, or nothing at all), the script exits silently

## License and credits

Distributed under the [MIT License](LICENSE).

Author: [Aleksei Vorobev / Patch34](https://github.com/patch-34).