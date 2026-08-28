# MmoWork

A small multiplayer game. This repository hosts the download only — there is no
source code here.

## Playing

1. Download **[MmoWork-windows.zip](../../releases/download/runtime-3/MmoWork-windows.zip)** (about 70 MB)
2. Unzip it somewhere you don't mind the game living
3. Run **`MmoWork.exe`**

That's the whole install. There's no installer, no launcher, and nothing to
configure — the server address is built in.

## Updates

The game checks while the login screen is up. If there's a new build, an
**Update** button appears at the bottom — press it and the game downloads what
changed, installs it, and restarts itself.

That download is normally well under a megabyte. The engine and .NET runtime
are the bulk of the install and only change when the engine does, so ordinary
updates only carry the map and the game code.

Nothing updates behind your back, and nothing updates while you're playing.

## What gets installed

| | |
|---|---|
| `MmoWork.exe` + `data_…` | the Godot engine and .NET runtime, ~181 MB unpacked |
| `MmoWork.pck` | the game world |
| `installed.json` | which build you're on |

Your account and characters are **not** stored here — they live on the server,
so they survive reinstalling, and they aren't yours to lose.

## Hosting your own

`Host.bat` runs the same build as a dedicated server. An account on your server
is yours alone; it doesn't exist on anyone else's.
