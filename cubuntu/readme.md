# 🐧 JSON-buntu

**A browser-based Ubuntu desktop simulation — no backend, no dependencies, just one `index.html`.**

Your entire OS (files, settings, windows, trash) lives in a single JSON state object. Save it to disk, load it back, and pick up exactly where you left off.

---

## Features

**Desktop Shell**
- Top bar with live clock, quick-settings panel (dark/light mode, volume, Wi-Fi)
- Ubuntu-style dock with open-app indicators — left on desktop, bottom on mobile

**Window Manager**
- Draggable, resizable windows via Pointer Events API (mouse, touch & stylus)
- Minimize, maximize, close controls
- Z-index focus management

**Applications**
| App | Highlights |
|---|---|
| Terminal | `ls`, `cd`, `cat`, `mkdir`, `touch`, `rm`, `echo > file`, `pwd`, `clear` + command history |
| File Manager | Breadcrumb nav, icon grid, rename, delete, opens files in Text Editor |
| Text Editor | Edit & save files directly into the JSON filesystem |
| Settings | Wallpaper (6 gradients), dark/light theme, username |
| Trash | Restore or permanently delete items |

**Touch & Mobile**
- Single tap = click, double-tap = open file/folder
- Touch-drag on title bar = window drag
- Long-press (500ms) = right-click context menu
- Fully responsive — dock and windows adapt to small screens

**Save / Load**
- Export OS state as `my-ubuntu.json` from the system tray
- Boot screen lets you load any saved `.json` disk image

---

## Usage

Just open `index.html` in any modern browser. No install, no server required.

```
open index.html
```

**Keyboard shortcuts**
- `Ctrl+T` — Open Terminal
- `Ctrl+E` — Open File Manager

---

## Tech Stack

Pure HTML5, CSS3, and vanilla JavaScript (ES6+). Zero external dependencies (Google Fonts only).
