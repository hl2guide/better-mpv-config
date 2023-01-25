# better-mpv-config

- Version: 1.0.9
- Last Updated (AEST): 2023-01-25 11:55:57PM

## What's New

- I've personally switched to MPV v3 since the Windows app and `updater.bat` has problems for v2.
- I've added a vastly simplified and elegant _mpv v3_ config file tested on [MPV v3 for Windows](https://sourceforge.net/projects/mpv-player-windows/files/64bit-v3/)

_Version 1.0.9_:
- Improved seeking
- Improved autohide
- Fixed input.conf playlist navigation

_Version 1.0.8_:
- Added mpv v3 config file

_Version 1.0.7_:
- Updated shaders (should improve performance)

_Version 1.0.6_ fixes:
- [profile restore actions](https://mpv.io/manual/stable/#configuration-files-copy-equal)

_Version 1.0.5_ added:
- meaningful profile descriptions
- an "alongside" optional mpv.conf (for users who want the config file next to mpv.exe)
- a hotfix for "alongside" config, fixed three paths

## Intro

This is an improved MPV Media Player configuration file (and shaders folder) that:

- has useful defaults
- hides the window title bar
- auto-hides the cursor after 1 second
- saves the seekbar position on exit
- uses an extra large RAM cache
- normalizes audio
- adds no additional cruft...

## Requirements

* official MPV Player: https://mpv.io/
* a PC with at least 4GB of RAM
* a PC with integrated (CPU) or discreet GPU (card)

![usage preview](https://raw.githubusercontent.com/hl2guide/better-mpv-config/master/preview%20image.png)

## Configuration for MPV v3

Just place the `mpv.conf` file next to `mpv.exe`.

## Configuration for older MPV v2

See [README](README_V2.md) for MPV v2.
