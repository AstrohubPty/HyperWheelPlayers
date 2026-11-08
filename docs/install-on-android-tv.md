# Install on Google TV and Android TV

_Install the HyperWheel Player app on Google TV, Android TV and Android TV boxes, using Downloader, Send Files to TV or ADB._

> **Tested on:** an Android 14 Google TV emulator, including the install screens, the settings panel with a remote, starting at boot and updating. It has not yet been tested on a physical TV or box. Menu names differ between makers and Android versions.

## What you need

- a Google TV, Android TV or Chromecast with Google TV device, or an Android TV box, running Android 7 or later
- an internet connection
- a way to get the file onto the TV: the Downloader app, Send Files to TV, or ADB

For Fire TV, see the separate Fire TV guide.

## 1. Allow installs from outside the Play Store

1. Open **Settings**, then **System**, then **About**.
2. Select **Android TV OS build** (or **Build**) seven times until a message says you are now a developer.
3. Go back to **Settings**, then **Apps**, then **Security & restrictions**, then **Unknown sources**. Turn on the app you will use to open the file (Downloader, or Files by Google).

On Android 8 and later, Android may ask you to allow this the first time you open the file instead.

## 2. Get the app onto the TV

Pick one.

**Downloader (the quickest with a remote)**

1. Install **Downloader** from the Google Play Store on the TV.
2. Open it and enter **hypr.onl/get** in the address bar. Select **Go**.
3. When the download finishes, select **Install**, then **Done**.

**Send Files to TV**

1. Install **Send Files to TV** on the TV and on your phone.
2. Send the file `HyperWheel-Player_latest_android.apk` from your phone to the TV.
3. Open the file on the TV and select **Install**.

**ADB**

1. In **Developer options**, turn on **USB debugging** (or **Wireless debugging**) and note the TV's IP address.
2. On a computer:

```sh
adb connect <tv-ip-address>:5555
adb install -r HyperWheel-Player_latest_android.apk
```

## 3. Open the app

Find **HyperWheel Player** in your apps row. It shows **Link this screen** with a QR code. Follow [Connect a device](https://docs.hyperwheel.app/screens/connect-a-device/) from the QR code step. Press **OK** on the remote to open the settings panel.

## Start on boot

**Launch on boot** is on by default. Android 10 and later also need **Display over other apps** for the app:

1. Open the settings panel and look under **Settings**. The **Display over other apps** row shows **Not allowed**.
2. Press **OK** on it. Android opens **Allow display over other apps**. Turn on **HyperWheel Player**, then press **Back**.

If a TV has no such screen, use ADB:

```sh
adb shell appops set app.hyperwheel.player SYSTEM_ALERT_WINDOW allow
```

The app also restarts by itself if it stops unexpectedly. It does this at most three times in ten minutes, so a repeating fault cannot keep the TV busy.

## Remote control

- **OK** opens the settings panel. The arrows move, **OK** selects.
- **Back** closes the panel one step at a time. With the panel closed, **Back** does nothing, so a stray press never leaves the player.
- To leave the app, **press and hold Back** for three seconds. **Home** also leaves it.
- If your remote has a **Menu** button, it opens the settings panel too.

## Update

The app checks for a new version every few hours. When one is ready, **Actions** shows a dot. Open **Actions**, select **Install**, and confirm with the remote. The first time, allow **Install unknown apps** for HyperWheel Player when Android asks.

## Uninstall

Open **Settings**, then **Apps**, select **HyperWheel Player**, then **Uninstall**.

## Troubleshooting

- **The first OK press does nothing straight after launch.** Press it again.
- **The app does not start after a power cut.** Allow **Display over other apps**, as above.
- **Video looks wrong or the app will not start on a box with an old system.** Open **Settings**, **Apps**, **Android System WebView**, and update it from the Play Store if you can. If the box cannot be updated, it is not supported.
- **The screen stays on Link this screen.** See [Connect a device](https://docs.hyperwheel.app/screens/connect-a-device/).
