# better-mpv-config

- Version: 1.3
- Last Updated (AEST): 2023-11-21 10:00:24PM
- Target Platform: Windows 10 or later (not tested on Apple or Linux at all)
- Test PC: New Intel i9 Desktop
    - CPU: Intel i9-13900K @ 3GHz
    - RAM: 64GB
    - GPU: NVidia GeForce RTX 4070 12GB
    - OS: Windows 11 Pro 23H2

## What's New

_Version 1.3 (Nov 21, 2023)_
- Changed default player behaviour to keep it open after a video/playlist ends
- Improved `input.conf` for easier seeking
- Updated `mpv.conf` to default base shaders `SSimDownscaler`, `SSimSuperRes`, `KrigBilateral` to off
    - I did this since in testing I noticed over-sharpening and ghosting
- Added easy activation of `uosc` in `mpv_osd.conf` (default is off)

See [HISTORY.md](HISTORY.md) for the history of older versions.

## Important Notes

⚠️ Be sure to customize `mpv_v3\mpv.conf` and `mpv_v3\input.conf` manually,
to make sure that the font and language are valid ⚠️

The defaults are:

- `Arial` for the subtitle font
- `en,eng` (English) for the audio and subtitle languages

As of version 1.1.00 please check the other `.conf` files as well.

📝 I suggest that you have a read of my __mpv.conf__ and alter it to your liking. 📝

- I've personally switched to MPV v3 since the Windows app and `updater.bat` has problems for MPV v2
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
- sets the default video, audio, and subtitle language to `en,eng`
- uses shaders to improve, upscale and downscale videos
    - CAS, FSR, KrigBilateral, SSimDownscaler and SSimSuperRes
- has been tested on Windows 10 and 11 only (not tested on Apple or Linux)
- adds no additional cruft...

## Requirements

* official MPV Player: https://mpv.io/ - [download MPV v3](https://sourceforge.net/projects/mpv-player-windows/files/64bit-v3/)
* a PC with at least 4GB of RAM (8GB or more recommended)
* a PC with integrated (CPU) or discrete GPU (card)

## Credits

* Some files are based off of the repo [Argon-/mpv-config](https://github.com/Argon-/mpv-config) by [Argon- (Julian)](https://github.com/Argon-)
* Inspired by [mpv-config](https://github.com/Zabooby/mpv-config) by [Zabooby](https://github.com/Zabooby)
* Shaders by [igv](https://gist.github.com/igv) and [agyild](https://gist.github.com/agyild/)

## Configuration for MPV v3

0. Download the [latest release](https://github.com/hl2guide/better-mpv-config/releases)
1. Extract the `configs` and `shaders` folders next to `mpv.exe`
2. Extract the `mpv.conf` and `input.conf` files next to `mpv.exe`
3. Delete `input.conf` if desired (custom keybindings)
4. In the `mpv.conf` file toggle the include line for the type of GPU you use (defaults to NVidia)
5. If your GPU cannot handle the shaders in `mpv.conf`, delete or comment out the include line for `configs\mpv_shaders.conf`
