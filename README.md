# better-mpv-config

- Version: 1.0.10
- Last Updated (AEST): 2023-04-05 11:13:00PM
- Platform: Windows 11 (not tested on Apple or Linux at all)

## What's New

- Removed legacy config file

_Version 1.0.10 (Feb 2023)_:
- Rewrote `mpv_v3\mpv.conf` and `mpv_v3\input.conf` (adapted from the repo [Argon-/mpv-config](https://github.com/Argon-/mpv-config))
- Vastly improved terminal, OSD, audio, subtitle, playback and playlist settings

⚠️ Be sure to customize `mpv_v3\mpv.conf` and `mpv_v3\input.conf` manually,
to make sure that the font and language are valid ⚠️

The defaults are:

- `Arial` for the subtitle font
- `en,eng` (English) for the audio and subtitle languages

See [HISTORY.md](HISTORY.md) for the history of older versions.

- I've personally switched to MPV v3 since the Windows app and `updater.bat` has problems for v2
- I've added a vastly better _mpv v3_ config file tested on [MPV v3 for Windows](https://sourceforge.net/projects/mpv-player-windows/files/64bit-v3/)

## Intro

This is an improved MPV Media Player v3 configuration file that:

- has useful defaults
- auto-hides the cursor after 200ms (when fullscreen)
- disables autoplay
- enables fast seeking
- improves OSD messages and style (moves progress bar to the top)
- saves the seekbar position on exit
- sets max volume (100%) and default volume (70%)
- sets subtitle font to `Arial` and sets the color to off-yellow
- sets the HLS bitrate to maximum
- sets the default audio language and subtitle language to `en,eng`
- has been tested on Windows 11 only (not tested on Apple or Linux)
- adds no additional cruft...

## Requirements

* official MPV Player: https://mpv.io/ - [download MPV v3](https://sourceforge.net/projects/mpv-player-windows/files/64bit-v3/)
* a PC with at least 4GB of RAM (8GB or more recommended)
* a PC with integrated (CPU) or discreet GPU (card)

## Credits

* Some files are based off of the repo [Argon-/mpv-config](https://github.com/Argon-/mpv-config) by [Argon- (Julian)](https://github.com/Argon-)

## Configuration for MPV v3

1. place the `mpv.conf` file next to `mpv.exe`
2. (Optional) for many changed keybindings, place the `input.conf` file next to `mpv.exe`
