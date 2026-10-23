# DiskFrontier

*Disk space — the final frontier.*

A fast, minimalist disk usage explorer for Windows: a single native executable with no dependencies. DiskFrontier 2 is a rewrite of the original DiskFrontier disk usage logger (Choice Computing, 1996–2001).

## Download

**[Download DiskFrontier.exe](https://github.com/paulusTheHub/diskfrontier-releases/releases/latest/download/DiskFrontier.exe)** (latest version, 64-bit, Windows 10 and 11). There is no installer: copy it anywhere and run it.

On the [releases page](https://github.com/paulusTheHub/diskfrontier-releases/releases/latest), the file to download is **DiskFrontier.exe** under *Assets*. The "Source code" zip files GitHub adds to every release contain only this README.

### First run

DiskFrontier is not yet code-signed, so the first time you run a downloaded copy Windows shows **"Windows protected your PC"** with only a *Don't run* button. Click **More info**, then **Run anyway**. Windows remembers the choice for that file.

Alternatively, before running it: right-click `DiskFrontier.exe` → **Properties** → tick **Unblock** → **OK**.

Settings are kept in the registry under `HKCU\Software\Choice Computing\DiskFrontier`, and saved indexes in `%LOCALAPPDATA%\DiskFrontier`.

## Features

- **Fast scans.** Run elevated, it reads the NTFS master file table directly (a whole drive with over a million files in a few seconds). Without admin rights it walks folders in parallel.
- **Instant start, live updates.** The index is saved between runs and, when elevated, kept current from the NTFS change journal. Options → *Always run elevated, no UAC prompt* sets this up once.
- **Tree with usage bars**: gray is size, the top half shows the share read recently and the bottom half the share written recently, over a window you choose.
- **Search** as you type across the whole drive; `*` and `?` wildcards work. Find files by date or hour too: `dm:10d`, `dm:3h`, `dm:2025`, `dm:2024-01-01..2024-03-31` (`da:` for last access), or pick dates with Ctrl+D. Recent searches are kept in a dropdown.
- **Treemap** (F9), cushion-shaded, colored by file type or by activity (F8), with a color key.
- Explorer right-click menu entry, drag and drop, delete to the Recycle Bin, recent folders.

This repository holds releases only.

---

Conceived and written by Paul Harper. Choice Computing 1996–2026.
