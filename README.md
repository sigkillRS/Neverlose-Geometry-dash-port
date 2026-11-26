# Neverlose Geometry Dash Port

A **Neverlose-style menu** for Geometry Dash x64. Independent, unofficial implementation by sigkill.

This project is not affiliated with or endorsed by Neverlose or the game developers. Use it only in private/offline play and respect the game's rules.

---

## Repository contents

The repository root contains two archives:

| File | What is inside |
| --- | --- |
| `Neverlose-Geometry-dash-port-v1.0.0_full.zip` | **Full package:** sources (`src\`, `vendor\`), `build.bat`, `resources.rc`, documentation, and ready-to-use binaries |
| `Neverlose-Geometry-dash-port-v1.0.0_binaries.zip` | **Ready-to-use package:** `build\StandaloneCheat.dll`, `build\Injector.exe`, `README.md`, `START_HERE_RU.txt`, licenses, and an example config |

The source code is intentionally kept inside `full.zip` instead of being expanded at the repository root. This keeps the repository small and lets you download the whole project as a single archive.

The ready-to-use binaries are also attached to the **v1.0.0** release:

- `StandaloneCheat.dll`
- `Injector.exe`

Release link (replace `<YOUR_USERNAME>` with your GitHub login):

```text
https://github.com/<YOUR_USERNAME>/Neverlose-Geometry-dash-port/releases/tag/v1.0.0
```

---

## What to download

| Goal | Get this |
| --- | --- |
| Just run and play | `Injector.exe` + `StandaloneCheat.dll` from the **Releases** section |
| Download everything in one file | `Neverlose-Geometry-dash-port-v1.0.0_binaries.zip` |
| Inspect or rebuild the code | `Neverlose-Geometry-dash-port-v1.0.0_full.zip` |

---

## Quick start

1. Download `Injector.exe` and `StandaloneCheat.dll` from the release, or extract `binaries.zip`.
2. Put both files **in the same folder**.
3. Run `Injector.exe` — it will find the game and inject the DLL automatically.  
   You can also run it manually:
   ```bat
   Injector.exe --launch
   ```
4. Wait for Geometry Dash to start.
5. In game:
   - **INSERT** — open/close the menu;
   - **X** — close the menu;
   - **LMB** — toggles, sliders, dragging the menu and overlays;
   - **RMB** on a row or badge — rebind a key.

> Antivirus software may flag injectors. This is expected for this kind of tool. Only add the folder to exclusions if you trust this build.

---

## Features

- Original-style canvas menu with animated tabs:
  **General**, **Visuals** (Players / World), **Unlocks**, **Misc**
- NL blue accent, fixed logo, enlarged rows and switches
- Draggable watermark and active-keybind list
- Right-click rebinding on rows and badges
- Three config slots: **Save Slot 1/2/3**, **Load Slot 1/2/3**
- Settings are stored in `nl_standalone.ini` next to the DLL
- Input blocking while the menu or overlays are active
- Cached page canvases with smooth tab transitions
- No loader, SDK, or mod manager required

---

## Configuration

`nl_standalone.ini` is created automatically next to `StandaloneCheat.dll` on first launch.

- Delete the file to reset everything to defaults.
- A ready example is included in both archives as `nl_standalone.example.ini`.
- Save slots are available on the **Misc** tab.

Default keybinds:

| Action | Key |
| --- | --- |
| Open/close menu | `INSERT` |
| Close menu | `X` |
| Noclip | `F1` |
| Godmode | `F2` |
| Jump Hack | `F3` |
| Speedhack | `F4` |
| Fly | `F5` |
| Hide Player | `F6` |
| Hitboxes | `F7` |
| Watermark | `F8` |

---

## Building from source

Extract `Neverlose-Geometry-dash-port-v1.0.0_full.zip`, then open **Developer Command Prompt for VS** and run:

```bat
cd "PATH\TO\EXTRACTED\FOLDER"
build.bat
```

Output:

```text
build\StandaloneCheat.dll
build\Injector.exe
```

Requirements:

- Windows x64
- Visual Studio 2022/2026 with **Desktop development with C++**
- Geometry Dash 2.2091 (x64)

ImGui, FreeType, fonts, and the canvas shell are already included in `vendor\`, so no internet connection is needed for the build.

---

## Archive verification

| Archive | SHA-256 |
| --- | --- |
| `Neverlose-Geometry-dash-port-v1.0.0_full.zip` | `949CAE0B20DB26E8AFDCFE5A1C25B08F30CEB3E6F2A576B3D4AACD9E8AD582EA` |
| `Neverlose-Geometry-dash-port-v1.0.0_binaries.zip` | `C7AF7A459B53D1B165F6265E13E7297B6E46CC456A74EDA8797334D04C535A7C` |

---

## License and credits

- Project code: **MIT**, `Copyright (c) 2026 barby`.
- Third-party components keep their own licenses — see `LICENSE` and `THIRD_PARTY_NOTICES.md` inside the archives.
- The visual style is a **Neverlose-style menu**. This is an independent implementation, not approved or supported by Neverlose or the game developers.
