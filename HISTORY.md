
_Version 1.3 (Nov 21, 2023)_
- Changed default player behaviour to keep it open after a video/playlist ends
- Improved `input.conf` for easier seeking
- Updated `mpv.conf` to default base shaders `SSimDownscaler`, `SSimSuperRes`, `KrigBilateral` to off
    - I did this since in testing I noticed over-sharpening and ghosting
- Added easy activation of `uosc` in `mpv_osd.conf` (default is off)

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
- Check out the new install instructions below (Configuration for MPV v3)

Version 1.1.10 (May 23, 2023)
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

_Version 1.0.12 (May 2023)_:
- Made videos start fullscreen on the primary screen
- Made the video window stay open after video playback (allows for drag and drop of video files)
- Added profiles for some file extensions (animations and static images)
- Removed legacy MPV v2 config file

_Version 1.0.10 (Feb 2023)_:
- Rewrote `mpv_v3\mpv.conf` and `mpv_v3\input.conf` (adapted from the repo [Argon-/mpv-config](https://github.com/Argon-/mpv-config))
- Vastly improved terminal, OSD, audio, subtitle, playback and playlist settings

_Version 1.0.9 (Jan 2023)_:
- Improved seeking
- Improved autohide
- Fixed input.conf playlist navigation

_Version 1.0.8 (Oct 2022)_:
- Added mpv v3 config file

_Version 1.0.7 (Jun 2022)_:
- Updated shaders (should improve performance)

_Version 1.0.6 (Feb 2022)_:
- [profile restore actions](https://mpv.io/manual/stable/#configuration-files-copy-equal)

_Version 1.0.5 (Jan 2022)_:
- meaningful profile descriptions
- an "alongside" optional `mpv.conf` (for users who want the config file next to mpv.exe)
- a hotfix for "alongside" config, fixed three paths
