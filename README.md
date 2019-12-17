# better-mpv-config
An improved MPV Player configuration file with useful defaults and profiles and no additional cruft.

Requires official MPV Player: https://mpv.io/

## Windows Users
Save to the file %APPDATA%/mpv/mpv.conf

## Linux Users
You can put all of the options in configuration files which will be read every time mpv is run.

The system-wide configuration file 'mpv.conf' is in your configuration directory (e.g. /etc/mpv or /usr/local/etc/mpv).

The user-specific one is ~/.config/mpv/mpv.conf.

## Usage

Save to the correct location (as above) for your Operating System.

Next time MPV is launched, and thereafter the settings should load. (command line or GUI)

## Vital Notes

If you run into playback issues then remove the first 5 lines and save changes to the file.

### Custom Profiles
This config uses specific naming convensions for shorter easier typing.

__Naming Convensions:__

L = Low, M = Medium, H = High

Low = 720p, Medium = 1080p, High = 2160p (4K)

30 = 30 frames per second, 60 = 60 frames per second

__Use the "profile" switch__

Windows e.g: mpv.exe --profile=H60

Windows e.g: mpv.exe --profile=M30

Linux e.g: mpv --profile=H60

Linux e.g: mpv --profile=M30
