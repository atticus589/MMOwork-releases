# MmoWork

A small multiplayer game. This repository hosts the download only — there is no
source code here.

## Playing

1. Download **`launcher.zip`** from [the latest release](../../releases/latest)
2. Unzip it somewhere you don't mind the game living — it will fill that folder
3. Run **`MmoWork-Launcher.exe`**

The first run downloads the game (about 70 MB) and starts it. After that the
launcher checks for updates each time and downloads only what changed, which is
usually well under a megabyte.

The server address is built in. There is nothing to configure.

## "Windows protected your PC"

You will probably see this the first time. The launcher isn't signed with a
code-signing certificate, and Windows warns about any unsigned program
downloaded from the internet regardless of what it does.

Click **More info**, then **Run anyway**.

If you'd rather not take that on faith, the launcher is about 300 lines and does
four things: ask this repository what the current build is, download it, check
its SHA-256, and start the game.

## What gets installed

| | |
|---|---|
| `MmoWork.exe` + `data_…` | the Godot engine and .NET runtime, ~181 MB unpacked |
| `MmoWork.pck` | the game world |
| `installed.json` | which build you're on, so unchanged files aren't downloaded again |

Your account and characters are **not** stored here — they live on the server.

## Updating

The launcher handles it. If it finds an update while the game is open it will
say so and ask you to close it — Windows won't let a running program have its
own files replaced.
