# Player settings and remote control

_Open the HyperWheel Player settings panel with a remote, keyboard, mouse or touch, and learn what each section does._

The settings panel slides in from the left of the player. Playback keeps running behind it. Everything in it works with a TV remote, a keyboard, a mouse or a touch screen.

## Open and close the panel

| How | To open | To close |
| --- | --- | --- |
| TV remote | Press **OK** (or **Select**, or **Menu** if your remote has it) | Press **Back** |
| Keyboard | Press **Enter** or **F2**, or **Ctrl+,** (**Command+,** on a Mac) | Press **Esc**, or **F2** again |
| Mouse | Move the pointer to the left edge for a moment, or click on the left edge | Click outside the panel, or the arrow at the top |
| Touch | Swipe in from the left edge | Swipe left |

The panel closes by itself after a minute with no input. Next time it opens at the section you used last.

## Move around

- **Up** and **Down** move between rows. **Left** and **Right** switch between the section list and the section, or change a value such as the theme.
- **OK** selects the highlighted row.
- **Back** goes up one step: from a section to the section list, then closed.
- On an Android TV or Fire TV, **Back** does nothing while the panel is closed. To leave the app, hold **Back** for three seconds.

## Sections

**Settings**

- **Theme:** system, light or dark.
- **Fullscreen:** on a computer, whether the player fills the screen.
- **On-screen debug:** shows connection and playback status over the content.
- **Launch on boot:** starts the player when the device starts.
- **Display over other apps:** on Android 10 and later, whether starting at boot is allowed.
- **Set PIN:** protects **Actions** with a 4 to 8 digit PIN.

**Actions**

- **Reload:** restarts the player page.
- **Clear cache:** downloads all content again.
- **Unlink this screen:** forgets the link code so the device can be linked to a different Screen. The Screen in HyperWheel is released at the same time.
- **Check for updates** and **Install:** see below.
- **Quit:** on a computer, closes the app.

**PWA, System and About** show information for support: the player version, whether it is online and connected, the Screen and organisation, the device model, system and web view version, memory and storage, and the app version. **About** also says whether this is a development, staging or production build. That is fixed when the app is built and cannot be changed in the app. **Copy diagnostics** puts all of it on the clipboard so you can paste it into a support message.

To turn on developer options, which add the server address to **About** and a **Remote server** setting that points this player at a different HyperWheel server (it unlinks the screen, so you link it again), open **About** and select the app version seven times.

## Protect the settings with a PIN

Under **Settings**, select **Set PIN** and enter 4 to 8 digits twice. From then on, opening **Actions** asks for the PIN, once each time the panel is opened. Five wrong tries lock the PIN for 30 seconds, and each further lock lasts longer.

**Forgot the PIN?** In HyperWheel, open the Screen's actions menu, then **Send command to screen**, then **Reset player PIN**. The Screen must be online. If it is offline, uninstall and reinstall the app (or clear its data), which also removes the PIN.

## Updates

- **Windows, macOS and Linux (AppImage):** automatic when the app starts.
- **Android, Google TV and Fire TV:** open **Actions**. A dot next to **Actions** means a new version is ready. Select **Install** and confirm in the Android prompt.

## Related

- [About the player app](about-the-player-app.md)
- [Connect a device](https://docs.hyperwheel.app/screens/connect-a-device/)
