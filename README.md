# DiskFrontier

*Disk space — the final frontier.*

A fast, minimalist disk usage explorer for Windows: a single native executable with no dependencies. DiskFrontier 2 is a rewrite of the original DiskFrontier disk usage logger (Choice Computing, 1996–2001).

## Download

Get `DiskFrontier.exe` from the **[latest release](https://github.com/paulusTheHub/diskfrontier-releases/releases/latest)**: a 64-bit build for Windows 10 and 11. There is no installer: copy it anywhere and run it. The exe is unsigned, so Windows SmartScreen may warn the first time you run it ("More info" → "Run anyway").

Settings are kept in the registry under `HKCU\Software\Choice Computing\DiskFrontier`, and saved indexes in `%LOCALAPPDATA%\DiskFrontier`.

## Features

- **Fast scans.** Run elevated, it reads the NTFS master file table directly (a whole drive with over a million files in a few seconds). Without admin rights it walks folders in parallel.
- **Instant start, live updates.** The index is saved between runs and, when elevated, kept current from the NTFS change journal. Options → *Always run elevated, no UAC prompt* sets this up once.
- **Tree with usage bars**: gray is size, the top half shows the share read recently and the bottom half the share written recently, over a window you choose.
- **Search** as you type across the whole drive; `*` and `?` wildcards work.
- **Treemap** (F9), cushion-shaded, colored by file type or by activity (F8), with a color key.
- Explorer right-click menu entry, drag and drop, delete to the Recycle Bin, recent folders.

This repository holds releases only.

---

Conceived and written by Paul Harper. Choice Computing 1996–2026.
