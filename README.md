# better-mpv-config
An improved MPV Player configuration file with:
- useful defaults
- profiles
- no additional cruft...

Requires official MPV Player: https://mpv.io/

## Configuration

### Windows Users
Save to the file %APPDATA%/mpv/mpv.conf

### Linux Users
You can put all of the options in configuration files which will be read every time mpv is run.

The system-wide configuration file 'mpv.conf' is in your configuration directory (e.g. /etc/mpv or /usr/local/etc/mpv).

The user-specific one is ~/.config/mpv/mpv.conf.

## Usage

Save to the correct location (as above) for your Operating System.

Next time MPV is launched, and thereafter the settings should load. (command line or GUI)

### Vital Notes

If you run into playback issues then remove the __first 5 lines__ and save changes to the file.

## Custom Profiles
This config uses specific naming convensions for shorter easier typing.

By default MPV plays video streams at the highest available quality.

Using my custom profiles allows for finer grain control over quality and framerate.

### Naming Convensions

Profiles use the format: \<letter\>\<number\>

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

## Examples

__Using the "profile" switch__

### Windows - 4K @ 60 FPS

mpv.exe --profile=U60

### Windows - 1080p @ 30 FPS

mpv.exe --profile=M30

### Linux - 4K @ 60 FPS

mpv --profile=U60

### Linux - 1080p @ 30 FPS

mpv --profile=M30
