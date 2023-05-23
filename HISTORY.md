
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
