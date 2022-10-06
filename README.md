# better-mpv-config

- Version: 1.0.8
- Last Updated (AEST): 2022-10-06 06:34:26PM

## What's New

- I've personally stopped using MPV v2 since the Windows app and `updater.bat` has problems
- I've added a vastly simplified and elegant _mpv v3_ config file tested on [MPV v3 for Windows](https://sourceforge.net/projects/mpv-player-windows/files/64bit-v3/)

_Version 1.0.8_:
- Added mpv v3 config file

_Version 1.0.7_:
- Updated shaders (should improve performance)

_Version 1.0.6_ fixes:
- [profile restore actions](https://mpv.io/manual/stable/#configuration-files-copy-equal)

_Version 1.0.5_ adds:
- meaningful profile descriptions
- an "alongside" optional mpv.conf (for users who want the config file next to mpv.exe)
- hotfix for "alongside" config, fixed three paths

## Intro

This is an improved MPV Media Player configuration file (and shaders folder) that:

- has useful defaults
- offers profiles
- hides the window title bar
- auto-hides the cursor after 1 second
- saves the seekbar position on exit
- uses an extra large RAM cache
- normalizes audio
- sets Color Space, Dithering, Debanding, Subtitles
- sets Motion Interpolation, Anti-Ringing and Upscaling & Processing
- now uses shaders for improved visuals
- improves profiles for https and http protocols
- adds no additional cruft...

## Credits

Thanks to all the original creators for making awesome shaders and extra work:

* [FSRCNNX](https://github.com/xzpyth/mpv-config/blob/main/shaders/FSRCNNX_x2_8-0-4-1.glsl)
* [KrigBilateral by Shiandow](https://gist.github.com/igv/a015fc885d5c22e6891820ad89555637)
* [SSimSuperRes by Shiandow](https://gist.github.com/igv/2364ffa6e81540f29cb7ab4c9bc05b6b)
* [SSimDownscaler by Shiandow](https://gist.github.com/igv/36508af3ffc84410fe39761d6969be10)

Includes selected lines from Mike Connelly's work on MPV.

* GitHub Repo: https://github.com/classicjazz/mpv-config
* Article: https://freetime.mikeconnelly.com/archives/5371

## Requirements

* official MPV Player: https://mpv.io/
* a PC with at least 4GB of RAM
* a PC with integrated (CPU) or discreet GPU (card)

![usage preview](https://raw.githubusercontent.com/hl2guide/better-mpv-config/master/preview%20image.png)

## Configuration for MPV v3

Just place the `mpv.conf` file next to `mpv.exe`.

## Configuration for older MPV v2

### Windows Users

Extract the ZIP in the releases section to the location: `%APPDATA%/mpv/`

### Linux Users

* You can put all of the options in configuration files which will be read every time mpv is run.
* The system-wide configuration file 'mpv.conf' is in your configuration directory (e.g. `/etc/mpv` or `/usr/local/etc/mpv`).
* The user-specific one is `~/.config/mpv/mpv.conf`.

### Mac Users

This config will need your own additional work if you happen to use a Mac PC (since Macs only support OpenGL).

I don't own any Mac PCs to test it so even if I wanted to I could not.

## Usage

* Extract to the correct location (as above) for your Operating System (pick between _mpv.conf_ and _alongside_, renaming to _mpv.conf_).
* Next time MPV is launched, and thereafter the settings should load. (command line or GUI)
* An initial seek time of 1 second is normal (tested on an old PC with 4 CPU cores) due to new shaders

### Vital Notes

If you run into playback issues then remove the __first 5 lines__ and save changes to the file 'mpv.conf'.

## Custom Profiles

This config uses specific naming convensions for shorter easier typing.

By default MPV plays video streams at the highest available quality (even 4K on a 1080p display).

Using my custom profiles allows for finer grain control over quality and framerate.

### Naming Convensions

Profiles use the format: `\<letter\>\<number\>`

The _letter_ referring to the video's __quality level__ and the _number_ the __FPS (frames per second)__.

| 480p | 720p | 1080p | 1440p (2.5K) | 2160p (4K) | 4320p (8K) |
| ------ | ------ | ------ | ------ | ------ | ------ |
| Very Low  | Low | Medium | High | Ultra | Supreme |

| Very Low  | Low | Medium | High | Ultra | Supreme |
| ------ | ------ | ------ | ------ | ------ | ------ |
| V | L | M | H | U | S |

| 30 FPS | 60 FPS |
| ------ | ------ |
| 30 | 60 |

(The config file now uses meaning descriptions so MPV's OSD and console will be more informative)

## Examples

__Using the "profile" switch__

#### Windows

4K @ 60 FPS:

`mpv.exe --profile=U60`

4K @ 30 FPS:

`mpv.exe --profile=U30`

1080p @ 60 FPS:

`mpv.exe --profile=M60`

1080p @ 30 FPS:

`mpv.exe --profile=M30`

#### Linux

Same as above but remove the `.exe` in the examples.
