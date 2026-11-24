# br-tv

A simplified **Channel Wall** launcher for Android TV / Fire TV, built from Bridge Music (`ru.bridgemusic.android`, v2.1.10).

The normal Bridge Music menus are stripped away. On launch you get **all channels as buttons** plus a single **Exit** button — a "channel wall". Pick a channel to play it fullscreen, use the arrows to zap between channels, and Back to return.

## Download

Grab the latest APK from **[Releases](../../releases)**, or download [`br-tv.apk`](br-tv.apk) directly from this repo.

- Size: ~12.5 MB
- Package: `ru.bridgemusic.android`
- Label shown on the home screen: **br-tv**
- Signed with a debug key (fine for sideloading; not a Play Store build)

## Install on a Fire TV / Fire Stick

**Over the network (ADB):**
```
adb connect <device-ip>:5555
adb install -r br-tv.apk
```

**On the device itself:** enable *Settings → My Fire TV → Developer options → Apps from Unknown Sources*, then open the APK with a sideload tool (e.g. Downloader app) pointed at the release link.

## Controls

| Where | Button | Action |
|-------|--------|--------|
| Channel wall | OK / center | Play the selected channel (fullscreen) |
| Channel wall | Back | Quit the app |
| Channel wall | Exit button | Quit the app |
| Playing | Left / Up | Previous channel |
| Playing | Right / Down | Next channel |
| Playing | Back | Stop playback, return to the channel wall |

The selected button shows an orange focus outline so you can always see where you are.

## What was changed vs. stock Bridge Music

- Start screen shows only channels + Exit (Главное / Новости / Чарты / О нас hidden)
- Bell / messages button hidden
- OK on a channel plays it fullscreen; arrows zap channels
- Back in the player fully stops playback and returns to the grid
- Back / Exit on the grid quits immediately (no confirmation dialog)
- Visible orange focus outline on the selected button
- App renamed to **br-tv**

## Notes

This is a personal modification for sideloading onto my own devices. Debug-signed universal APK (works on both Android TV boxes and Fire TV).
