# better-mpv-config

- Version: 1.3
- Last Updated (AEST): 2023-11-21 09:20:39PM
- Target Platform: Windows 10 (not tested on Apple or Linux at all)
- Test PC: New Intel i9 Desktop
    - CPU: Intel i9-13900K @ 3.50GHz
    - RAM: 64G
    - GPU: NVidia GeForce GTX 4060 12GB
    - OS: Windows 11 Pro 23H2

## Upcoming

Version 1.3 may be ready before the end of December.

It is slated to include useful fixes, better defaults and some cleanup.

## What's New

_Version 1.3 (Nov 21, 2023)_
- Improved `input.conf` for easier seeking
-

_Version 1.2.1 (Sept 27, 2023)_
- Split shaders into two sets (big improvement to quality of GPU shaders)
    - NVidia
    - AMD and Intel
- Improved `input.conf`
    - new keys for playback speed
    - upscaler shader mode

_Version 1.1.25 (Aug 13, 2023)_
- Fixed all console messages and implemented stricter MPV pathing for HOME_PATH
- Improved optional `input.conf` with quiet mode seeking and other minor changes
- Disabled `hwdec` for the moment while MPV seems to enable it by default
- Check new install instructions below (Configuration for MPV v3)

_Version 1.1.10 (May 23, 2023)_
- HOTFIX: Fixed upscaler shaders to only apply to videos lower than 1080p

_Version 1.1.00 (May 23, 2023)_
- Added shaders
    - SSimDownscaler by [igv](https://gist.github.com/igv/36508af3ffc84410fe39761d6969be10)
    - SSimSuperRes by [igv](https://gist.github.com/igv/2364ffa6e81540f29cb7ab4c9bc05b6b)
    - KrigBilateral by [igv](https://gist.github.com/igv/a015fc885d5c22e6891820ad89555637)
    - Nvidia Adaptive-directional sharpening algorithm shader by [agyild](https://gist.github.com/agyild/7e8951915b2bf24526a9343d951db214)
    - Contrast Adaptive Sharpening (CAS) by [agyild](https://gist.github.com/agyild/bbb4e58298b2f86aa24da3032a0d2ee6)
    - FidelityFX Super Resolution (FSR) by [agyild](https://gist.github.com/agyild/82219c545228d70c5604f865ce0b0ce5)
- Split config file into six files (organized and easier toggling)

## Important Notes

⚠️ Be sure to customize `mpv_v3\mpv.conf` and `mpv_v3\input.conf` manually,
to make sure that the font and language are valid ⚠️

The defaults are:

- `Arial` for the subtitle font
- `en,eng` (English) for the audio and subtitle languages

See [HISTORY.md](HISTORY.md) for the history of older versions.

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
