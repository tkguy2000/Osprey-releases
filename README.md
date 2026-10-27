# Osprey

**English** | [한국어](README.ko.md)

**[⬇ Download the latest version](https://github.com/tkguy2000/Osprey-releases/releases/latest)** — get `Osprey-Setup-x.y.z.exe` and run it.

---


Osprey is a Windows file explorer for photos, videos and archives. You can view them in one window, organize them with ratings, tags and notes, and find them fast.
Your files stay on your PC. Nothing is uploaded anywhere.

## 1. Install

1. Download the latest `Osprey-Setup-x.y.z.exe` and run it. It installs into your user folder (no admin rights needed) and adds Start menu and desktop shortcuts.
2. If a blue **Windows SmartScreen** warning appears the first time, click **More info → Run anyway**. The app isn't code-signed yet, which is why Windows warns.
3. To use it without installing, unzip `OspreyExplorer-win-Portable.zip` and run `Osprey.exe`.

- Requires Windows 10/11, 64-bit.
- On first launch you choose the language (English or Korean). You can change it later in **⚙ → Settings…**.
- The window title shows the current version, e.g. `Osprey 0.1.27`.

### Updates
Osprey checks for a new version every time it starts (no account or token needed). When one is available it asks first. Click yes and it downloads, then restarts. It never installs silently.
You can also check by hand: **⚙ → Updates… → Check now → Download and restart**.

## 2. Getting started

1. Click **+ Folder** above the list and add the folders you use most (photos, videos, projects…). You can add as many as you like.
2. The first time, Osprey asks **where to keep thumbnails**. Pick a folder on a drive with free space. Folders inside your library aren't allowed.
3. The folder shows up in the left pane right away. Even a huge folder is usable quickly, because Osprey reads the file list first and does the rest in the background.

## 3. The window

| Pane | What it does |
|---|---|
| **Preview** | Shows the selected photo, video or archive. Tabs along the top also open web pages (YouTube and others). |
| **Browse** | Your library folders plus smart categories: ratings, labels, tags, recently viewed and more. Click one to show it in the list. |
| **List** | The folders and files in the current location. Double-click a folder to go in. Use `..` at the top or Backspace to go up. |
| **Notes** | Click the arrow on the right edge to open it. It lists every file you've attached a note to. |

### Rearranging panes
- Drag a pane's title tab onto the top, bottom, left or right side of another pane to split it. Drop it in the middle to merge the two as tabs.
- Each pane has a **⋯** menu with these items:
  - Split up, down, left or right (opens a second list on the same folder).
  - Maximize, Collapse, Restore sizes.
  - Close.
- If the layout gets messy, use **⋯ → Reset panels** or **⚙ → Settings… → Reset panels**.
- Your layout is saved when you close Osprey and comes back the next time.

## 4. Working with the list

### Address bar and search
- The address bar above the list shows where you are. Paste a folder path and press Enter to go there.
- Click **🔍** (or press Ctrl+F) to turn the same box into a search box. Click it again or press Esc to get the address back.
- **⟳** refreshes only the current folder. To re-read the whole library, use **⚙ → Rescan the whole library (slow)**.
- Opening a folder quietly syncs it in the background, picking up files that were added or deleted outside Osprey.

### Views
- Choose a view from **View ▾**:
  - **Tiles**: large thumbnails, with adjustable size.
  - **Wide**.
  - **Compact**: one line per file.
  - **Details**: name, date, type and size only, without thumbnails.
- The same row has the kind filter (all, photos, videos, archives…), the sort order (name, date, size, rating…) and ↓ to flip ascending or descending.
- Thumbnails fill in one by one, starting with the folder you're looking at. Move to another folder and that folder goes first.
- Some files can't have a thumbnail:
  - Text files (txt, md, log, json…) show their first lines.
  - Anything else (Houdini .hip files, for example) shows the same icon Windows Explorer does.
- On video tiles, the red bar shows **how much you've watched**, and **✓ Watched** marks videos you finished.
- Move the mouse left and right over a video thumbnail to skim through its scenes.

### Organizing
| Action | How |
|---|---|
| Rating 0–5 | Number keys 0–5 |
| Color label | Ctrl+1–6 (Ctrl+0 clears) |
| Tag | T |
| Note (sticky note) | N, or right-click → Add/edit note. Files with notes show a yellow note in the top-right corner |
| Rename / batch rename | F2 / Shift+F2 |
| Delete | Del. This moves the file to Osprey's trash, and **Ctrl+Z** brings it back |
| Copy / cut / paste | Ctrl+C / Ctrl+X / Ctrl+V. Works back and forth with Windows Explorer |
| New folder / properties | Ctrl+Shift+N / Alt+Enter |
| Hide | H. Moves the file into the **Hidden vault**, out of sight. You set a PIN the first time, and Osprey asks for it when you open the vault |

- Click a note in the Notes pane to jump to that file's folder with the file selected.
- **Dual pane (F9)** shows two lists side by side. Drag files between them to move them, or hold Ctrl while dropping to copy.

## 5. Finding files

Type part of a name in the search box (🔍) to search the current folder and its subfolders. You can also combine these filters:

| Example | Meaning |
|---|---|
| `*.jpg` `ext:mp4;mov` | File extension |
| `size:>100mb` | Size |
| `dm:today` `dm:2026-10` | Date modified |
| `path:trip` | Text in the folder path |
| `rating:>=4` | Rated 4 or higher |
| `tag:family` `label:red` | Tag or color label |
| `played:` | Videos you've played |
| `dupe:` | Duplicate files |
| `regex:^IMG_\d+` | Regular expression |

- You can save searches you use often and run them again later.
- The **PC** button searches your whole PC. This needs [Everything](https://www.voidtools.com/) to be running.
- **⚙ → Find similar images…** groups look-alike photos and videos so you can clean them up.

## 6. Photos

- Select a photo to see it large in the Preview pane. Press **Space** for a Quick look window.
- Mouse wheel goes to the previous or next photo, and Ctrl + wheel zooms. While zoomed in, drag to pan.
- **F5** starts a slideshow and **F11** goes full screen. Press Esc to exit either.

## 7. Videos

Double-click a video or press Enter to play it in the Preview pane. It picks up where you left off.

| Control | Button / key |
|---|---|
| Play / pause (↻ replays after the end) | ▶ ⏸ ↻ / Space, or click the video |
| Back or forward 10 s / 1 s / one frame | −10s +10s / ← → / Shift+← → / , . |
| Previous / next video (list order) | ⏮ ⏭ / Ctrl+← → |
| Speed | Speed button menu / [ ] (\ resets to normal) |
| Repeat: off → this video → play next when done | 🔁 / L |
| Volume / mute | Slider, mouse wheel, ↑ ↓ / 🔊 or M |
| Full screen | ⛶ / F / double-click the video. Esc exits |
| Save scene (bookmark) / previous or next scene | ♥ / B / PgUp PgDn |
| Subtitle and audio tracks, subtitle sync, aspect ratio | ⋯ menu |

- Drag left or right across the video to scrub to a new position.
- You can give a saved scene an end point and loop that section.

## 8. Archives

- Open a zip, rar or 7z file to see the files and photos inside without extracting it. You can extract it too.
- For an archive full of images, use **Read as comic**:
  - Turn pages with ← →, Space or a click.
  - D shows two pages at a time.
  - R flips the reading direction.

## 9. Web tabs (YouTube and more)

- Click **+** at the top of the Preview pane to open a web tab, then type an address or a search. The **YouTube** button opens a YouTube tab.
- You can sort tabs into **groups** (for example Work and Personal). Click a group to see only its tabs.
  - Right-click a tab to move it to a group or to a new group.
  - Right-click a group to rename it, change its color or delete it.
- Open tabs and groups come back next time, and YouTube videos resume where you stopped.

## 10. Settings and tools (⚙ menu)

- **Settings…**: language, theme, thumbnail location, thumbnail size, clearing thumbnails, and reset panels.
- **Shortcuts…**: change any keyboard shortcut. Osprey warns you about conflicts.
- **Updates…**: check for and install a new version. You can turn the startup check on or off here.
- **Folder sizes…**: see at a glance which folders take up the most space.
- **Removing a folder from the library**: right-click it in the Browse pane and choose remove.
  - This clears only Osprey's records for that folder (ratings, tags, notes) and its thumbnails. **Your actual files are not touched.**
  - If the folder still has hidden files, unhide them first.

## 11. Safety

- Files you delete in Osprey aren't erased. They move into that folder's `.osprey\trash`, and **Ctrl+Z** undoes the delete.
  "Empty trash" sends them to the Windows Recycle Bin, so you can still restore them from there.
- Osprey never writes outside the folders you added to the library, except thumbnails, which go only in the location you chose.
- Uninstalling keeps your ratings, tags and notes, so if you reinstall you pick up where you left off.
  If you have hidden files, unhide them in Osprey before uninstalling.

| What | Where |
|---|---|
| Program | `%LocalAppData%\OspreyExplorer` |
| Ratings, tags, notes | `%LocalAppData%\Osprey` |
| Settings | `%AppData%\Osprey\settings.json` |
| Thumbnails | `OspreyCache` inside the folder you chose |

## 12. For testers

If something goes wrong, please send:
- The version from the window title (e.g. `Osprey 0.1.27`).
- What you were doing and what happened. A screenshot helps, but please blur any private file names.
- If Osprey crashed or froze, the `crash-<date>.log` or `hang-<date>.log` file from `%LocalAppData%\Osprey\logs`.
