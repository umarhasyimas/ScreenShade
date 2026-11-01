<div align="center">

# Pot-O ScreenShade

**A gentle screen color filter, blue-light reducer and screenshot tool for Windows.**

![Platform](https://img.shields.io/badge/platform-Windows%2010%20%2F%2011%20(64--bit)-0078D6)
![License](https://img.shields.io/badge/license-Freeware-FF9A3D)
![Privacy](https://img.shields.io/badge/network-none%20%E2%80%A2%20no%20telemetry-4CC38A)

[Download](https://github.com/umarhasyimas/ScreenShade/releases) ·
[Report a problem](https://github.com/umarhasyimas/ScreenShade/issues) ·
[License](#license)

</div>

---

## What is it?

Pot-O ScreenShade lays a soft, adjustable color tint over your whole screen so late-night work is easier on the eyes. It can warm up the colors, reduce blue light, or cover the screen with any color you like. It also includes a built-in screenshot tool with simple annotation, so you do not need a second program for quick captures.

It is small, runs quietly in the system tray, works completely offline, and is **free**.

> **Note:** ScreenShade is a visual tint drawn over your screen. It does not change your monitor's hardware or backlight, and it makes no medical claims about eye health or sleep.

## Features

### Screen filter
- **One-click looks:** Daylight, Reading, Evening, Night, Deep Night, plus a Custom look that remembers your last manual settings.
- **Three simple sliders:**
  - **Color warmth:** from cool bluish-white to warm orange.
  - **Overlay opacity:** how strongly the tint covers the screen.
  - **Blue-light filter (Intensity):** an extra amber layer that reduces blue light. 0% means off.
- **Custom color mask:** pick any color with the color picker, type a HEX code, choose from ready-made swatches, and reuse recently used colors.
- **Live preview** of the tint, and every change applies instantly. There is no Apply button.
- **Gentle by default:** first launch starts with a soft setting (5000K, 10% opacity, 15% blue-light).
- **Master switch** in the header and tray: turns the whole filter (color and blue-light) on or off together.
- **Multi-monitor support:** every connected display is covered.
- **Click-through and focus-free:** the overlay never blocks your mouse, never steals keyboard focus and never shows up in Alt+Tab.

### Screenshots
- **Choose what to capture:** press **Print Screen** (or the Screenshot button) and pick **Selected area** or **Entire screen**.
- **Lightshot-style selector:** drag to select, then move or resize the selection with handles. A live size readout is shown.
- **Annotation tools:** rectangle, arrow, line, pencil, text, highlighter and blur (pixelate), with a color palette, line thickness, **undo** and **redo**.
- **Copy, save or save as:** copy to the clipboard, save instantly, or choose a name and folder.
- **PNG or JPG**, with automatic names like `ScreenShade_20260101_203015.png`. Existing files are **never overwritten**.
- **Tint-free screenshots:** by default the color filter is hidden for a split second while capturing, so your saved image shows normal colors. You can switch this off if you want the tinted look.
- **Optional automatic screenshots** at a fixed interval (off by default).
- **Print Screen is your choice:** hand the plain Print Screen key back to Windows at any time, and use `Ctrl+Print Screen` / `Shift+Print Screen` for ScreenShade instead.

### Time and automation
- **Pause for 30 minutes** and the filter comes back by itself.
- **Timer:** choose a duration (5 min to 24 h) and what happens at the end: turn the filter on or off, restore your previous settings, switch to a preset, show a notification, or exit the app.
- **Daily schedule:** for example, apply *Evening* at 18:00 and *Deep Night* at 23:00.

### Everyday comfort
- **System tray app** with a clearly grouped menu (screen filter settings are greyed out while the filter is off, so you always know what affects what).
- **Global shortcuts** that work even when the window is hidden.
- **Start with Windows** (optional) and **start minimized to the tray**.
- **Emergency off** shortcut that instantly removes the tint.
- **Safe by design:** if the app ever closes or crashes, the tint disappears with it. It cannot get "stuck" on your screen.
- **Single instance:** launching it again simply brings the existing window forward.
- **Modern dark interface** with smooth animated controls.

## Download and install

1. Go to the **[Releases](https://github.com/umarhasyimas/ScreenShade/releases)** page.
2. Download **`PotO-ScreenShade-Setup-<version>-x64.exe`**.
3. Run it and follow the wizard.

**No administrator rights are needed.** The app installs for your Windows account only, to:

```
%LOCALAPPDATA%\Programs\Pot-O ScreenShade
```

During setup you can add Start Menu and desktop shortcuts. Upgrading to a newer version keeps your settings.

> **Windows SmartScreen:** because this is an independent, unsigned program, Windows may show "Windows protected your PC" the first time. Choose **More info → Run anyway** if you downloaded it from this repository.

### System requirements
| | |
|---|---|
| **OS** | Windows 10 (version 1809 or newer) or Windows 11 |
| **Architecture** | 64-bit only |
| **Admin rights** | Not required |
| **Internet** | Not required |

### Uninstall
Use **Settings → Apps → Installed apps → Pot-O ScreenShade → Uninstall** (or the uninstall shortcut in the Start Menu). You will be asked whether to keep your settings file. Your screenshots are never touched.

## Quick start

1. Launch **Pot-O ScreenShade**.
2. Under **1 · Pick a look**, click a preset such as **Evening**.
3. Optional: under **2 · Fine-tune**, adjust warmth, opacity and blue-light to taste.
4. Close the window. The filter keeps running from the system tray.
5. Right-click the tray icon any time to change settings, take a screenshot or exit.

## Keyboard shortcuts

All of these can be changed in **Settings → Shortcuts**.

| Action | Default |
|---|---|
| Turn the screen filter on / off | `Ctrl` + `Alt` + `O` |
| **Emergency filter off** | `Ctrl` + `Alt` + `Shift` + `O` |
| Screenshot (asks: area or entire screen) | `Print Screen` |
| Screenshot: selected area directly | `Ctrl` + `Print Screen` |
| Screenshot: entire screen directly | `Shift` + `Print Screen` |

**Inside the screenshot editor**

| Action | Keys |
|---|---|
| Copy to clipboard | `Ctrl` + `C` or `Enter` |
| Save | `Ctrl` + `S` |
| Undo / Redo | `Ctrl` + `Z` / `Ctrl` + `Y` |
| Cancel | `Esc` |

## How the tint works

The overlay is built from two independent layers:

1. **Color tint:** its color comes from the **Color warmth** slider *or* from a **custom color** you pick. **Overlay opacity** sets how strong it is.
2. **Blue-light layer:** a warm amber layer controlled only by the **Intensity** slider.

Because they are independent, you can use a strong tint with no blue-light layer, a pure blue-light filter with the tint at 0%, or any mix.

## Settings and your data

- **Settings** are saved automatically to `config.json` in the program folder. Invalid or damaged values are replaced with safe defaults.
- **Screenshots** are saved to `Pictures\ScreenShade` unless you choose another folder.
- **Privacy:** ScreenShade works entirely on your computer. It does not connect to the internet, collect data or send telemetry.

## Troubleshooting

<details>
<summary><b>The Print Screen key does nothing</b></summary>

Windows may be using it for the Snipping Tool. Turn that off in **Windows Settings → Accessibility → Keyboard → "Use the Print screen button to open screen capture"**. Another option is to use `Ctrl+Print Screen` or `Shift+Print Screen`, which ScreenShade can use without conflicts.
</details>

<details>
<summary><b>I want to use Windows' normal Print Screen</b></summary>

Untick **Use Print Screen key for ScreenShade** in the tray menu or in **Settings → Shortcuts**. The key returns to Windows immediately.
</details>

<details>
<summary><b>I want to take a screenshot of ScreenShade itself</b></summary>

By default the app hides its own window while capturing. Untick **Hide ScreenShade's own window while taking a screenshot** in **Settings → Screenshot**.
</details>

<details>
<summary><b>My screenshots have no color tint</b></summary>

That is intentional by default. Untick **Hide the screen filter tint from screenshots** in **Settings → Screen filter** if you want screenshots to look exactly like your tinted screen.
</details>

<details>
<summary><b>The tint is stuck or I can't reach the window</b></summary>

Press `Ctrl + Alt + Shift + O` for an instant emergency off, or right-click the tray icon and choose **Exit ScreenShade**.
</details>

<details>
<summary><b>The tint does not cover a game or video</b></summary>

Like all overlay-style filters, it cannot draw over some exclusive full-screen games or protected video playback. Running the game in borderless-windowed mode usually works.
</details>

<details>
<summary><b>Something else looks wrong</b></summary>

Please [open an issue](https://github.com/umarhasyimas/ScreenShade/issues) and include your Windows version, whether you use several monitors or display scaling, and what you were doing when it happened.
</details>

## License

Pot-O ScreenShade is **freeware**, released as a **binary only**, under the *Pot-O ScreenShade Freeware License* (see [`LICENSE.txt`](LICENSE.txt) in the installer and the program folder).

In short:

- ✅ Free to use on any number of your own computers, for personal or business use.
- ✅ Free to redistribute the complete, unmodified installer, as long as the license and credits stay intact and no fee is charged.
- ❌ No selling, renting or repackaging.
- ❌ No modification, reverse engineering or removal of credits.
- The software is provided "as is", without warranty.

The summary above is for convenience only. The full license text is what applies.

## Credits

**Created by Muhammad Umar Hasyim Ashari**

Copyright © 2026 Muhammad Umar Hasyim Ashari. All rights reserved.

### Third-party software

ScreenShade is built with these open-source projects, each under its own license (details in `THIRD_PARTY_NOTICES.txt`):

| Component | License |
|---|---|
| [Qt for Python (PySide6)](https://www.qt.io/qt-for-python) and Qt | LGPLv3 |
| [Python](https://www.python.org/) | PSF License |
| [Pillow](https://python-pillow.org/) | MIT-CMU (HPND) |
| [python-mss](https://github.com/BoboTiG/python-mss) | MIT |
| [pywin32](https://github.com/mhammond/pywin32) | PSF License |

Qt is dynamically linked: its libraries ship as separate files in the program folder. Qt is a registered trademark of The Qt Company Ltd.

---

<div align="center">

Made with care by **Muhammad Umar Hasyim Ashari** · [github.com/umarhasyimas/ScreenShade](https://github.com/umarhasyimas/ScreenShade)

</div>
