# MmoWork

A small multiplayer game. This repository hosts the download only — there is no
source code here.

## Playing

1. Download **`launcher.zip`** from [the latest release](../../releases/latest)
2. Unzip it somewhere you don't mind the game living — it will fill that folder
3. Run **`Play MmoWork.bat`**

The first run downloads the game (about 70 MB) and starts it. After that the
launcher checks for updates each time and downloads only what changed, which is
usually well under a megabyte.

The server address is built in. There is nothing to configure.

## If Windows or your antivirus complains

The launcher is a PowerShell script rather than a compiled program, and
"a batch file that runs PowerShell that downloads a zip" is a shape that
security software is reasonably suspicious of. Both files are plain text — 
`launcher.ps1` is readable in Notepad if you'd like to see exactly what it does
before running it.

## What gets installed

| | |
|---|---|
| `MmoWork.exe` + `data_…` | the Godot engine and .NET runtime, ~181 MB unpacked |
| `MmoWork.pck` | the game world |
| `installed.json` | which build you're on, so updates can be skipped when nothing changed |

Your account and characters are **not** stored here — they live on the server.
