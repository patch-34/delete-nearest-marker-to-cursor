# Patch34: Delete Nearest Marker to Cursor

Scripts and tools for REAPER. Useful, weird, and everything in between.

---

Deletes the marker closest to the edit cursor by absolute distance. Regions are ignored — markers only.

## Installation

1. In REAPER: **Actions → Show action list…**
2. Click **ReaScript: Load…**
3. Select `Patch34_Delete_Nearest_Marker_To_Cursor.lua`
4. Optionally assign a keyboard shortcut

## How it works

The script scans all project markers, calculates `abs(marker_pos - cursor_pos)` for each one, and deletes the nearest. The action is fully undoable.

## Notes

- Regions are skipped entirely
- If the project has no markers (only regions, or nothing at all), the script exits silently

## License

MIT
