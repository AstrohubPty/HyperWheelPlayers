# About the player app

_What the HyperWheel Player app is, which devices it supports, and how to download and install it._

The HyperWheel Player app runs your Screen's content full screen on a computer, an Android device or a TV. It is the same player you get by opening [hypr.onl](https://hypr.onl) in a browser, wrapped in an app that can start by itself, stay on top, and show a settings panel you can control with a TV remote.

You do not need the app to use HyperWheel. A browser works for many setups. Use the app when the device should start playing on its own after a power cut, when it has no keyboard or mouse, or when you want to manage it with a remote control.

## Supported devices

| Device | Install guide | Status |
| --- | --- | --- |
| Windows 10 (1809 or later) and Windows 11 | Install on Windows | Built, not yet tested on a Windows PC |
| macOS 12 or later, Intel and Apple Silicon | [Install on macOS](https://docs.hyperwheel.app/player-app/install-on-macos/) | Tested on a Mac |
| Debian, Ubuntu, Fedora and Raspberry Pi OS | [Install on Linux](https://docs.hyperwheel.app/player-app/install-on-linux/) | Packages tested in containers, not yet on hardware |
| Android phones and tablets | [Install on Android](install-on-android.md) | Tested on an emulator |
| Google TV and Android TV | [Install on Google TV and Android TV](install-on-android-tv.md) | Tested on an emulator, not yet on a TV |
| Fire TV (Fire OS 7 and later) | Install on Fire TV | Built, not yet tested on a Fire TV |
| ChromeOS | Install on ChromeOS | Built, not yet tested on a Chromebook |

**Only the Android app is available to download for now.** The Windows, macOS and Linux apps are not released yet.

Android devices need Android 7 or later. Older Fire TV models (Fire TV Stick 1st and 2nd generation, and any device on Fire OS 5) cannot run the app.

Guides marked "not yet tested" are published only when someone has followed them on the device. Until then, treat them as untested.

## Download the app

Download from the **Player apps** page in HyperWheel, which highlights the right file for your device. On a TV you can type a short address instead: **hypr.onl/get**. On an Android device it downloads the app directly. Anywhere else it opens the list of downloads.

Every download is published on the [HyperWheel Player releases page](https://github.com/AstrohubPty/HyperWheelPlayers/releases/latest), together with a `SHA256SUMS.txt` file. To check a download, compare its SHA-256 checksum with the one listed there.

## Why you see a security warning

The app is not yet signed with a Windows or Apple developer certificate, so Windows SmartScreen and macOS Gatekeeper warn before the first run. The install guides show how to continue. The warning is about the missing certificate. It does not mean the file is damaged. If you are unsure, check the file's checksum first.

Android shows its own prompt the first time you install an app from outside the Play Store.

## Link the screen

After installing, open the app. It shows **Link this screen** with a QR code and a device code. Follow [Connect a device](https://docs.hyperwheel.app/screens/connect-a-device/) from the QR code step.

## Start on boot

**Launch on boot** is on by default. On Android 10 and later, starting at boot also needs **Display over other apps** to be allowed for HyperWheel Player. The Settings panel shows whether it is allowed and opens the right Android screen for you.

## Updates

- **Windows, macOS and Linux:** the app checks for a new version when it starts and installs it automatically.
- **Android, Google TV and Fire TV:** the app checks every few hours. When a new version is ready, **Actions** in the settings panel shows a dot and an **Install** row. Android asks you to confirm the install. Nothing interrupts playback until you choose to install.

## Related

- [Player settings and remote control](player-settings.md)
- [Connect a device](https://docs.hyperwheel.app/screens/connect-a-device/)
- [Screen offline](https://docs.hyperwheel.app/troubleshooting/screen-offline/)
