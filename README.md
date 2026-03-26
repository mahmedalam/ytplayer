# YT Player

**A free, open-source video and audio player with a clean, modern UI — built with Python and PyQt6.**

![YT Player Preview](preview.svg)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/Python-3.14%2B-blue)](https://www.python.org/)
[![PyQt6](https://img.shields.io/badge/PyQt6-6.10.2-green)](https://pypi.org/project/PyQt6/)
[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux-lightgrey)](#)
[![Code Signing](https://img.shields.io/badge/Code%20Signing-SignPath%20Foundation-orange)](https://signpath.org)

---

## Downloads

| Platform | Link |
|----------|------|
| 🪟 Windows | [Download for Windows](#) |
| 🐧 Linux | Coming soon |

> **Security note:** The Windows `.exe` installer is digitally signed. See the [Code Signing Policy](#code-signing-policy) section below for details.

---

## Features

- 🤩 **Stylish, colorful UI** — a polished interface that feels great to use
- 🔥 **GPU rendering** — smooth, high-quality video playback
- <img src="https://cdn.icon-icons.com/icons2/1488/PNG/512/5314-windows_102509.png" height="16"> <img src="https://cdn.icon-icons.com/icons2/195/PNG/256/OS_Linux_23399.png" height="16"> **Cross-platform** — runs on Windows and Linux

---

## Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `Space` | Play / Pause |
| `←` | Rewind 5 seconds |
| `→` | Forward 5 seconds |
| `↑` | Volume up |
| `↓` | Volume down |
| `M` | Toggle mute |
| `F` | Toggle full screen |
| `Q` | Quit |

---

## Installation

### Option 1 — Download a release (recommended)

Download the installer or portable executable from the [Downloads](#downloads) section above.

### Option 2 — Run from source

**Requirements:** Python 3.14+

```bash
# Clone the repository
git clone https://github.com/mahmedalam/ytplayer.git
cd ytplayer

# Install dependencies
pip install -r requirements.txt

# Launch the player
python main.py
```

To open a specific file directly:

```bash
python main.py /path/to/your/video.mp4
```

### Option 3 — Build your own executable

The project uses [PyInstaller](https://pyinstaller.org/) for packaging.

```bash
pip install pyinstaller
pyinstaller --onefile --windowed --icon="YT Player.ico" main.py
```

The compiled executable will be in the `dist/` folder.

---

## Project Structure

```
ytplayer/
├── main.py              # Application entry point & main window
├── interface.py         # UI layout and widget setup
├── custom_widgets.py    # Custom PyQt6 widgets
├── style.py             # Application stylesheet (CSS-in-Python)
├── shortcuts.py         # Keyboard shortcuts dialog
├── author.py            # Author info dialog
├── fonts.py / font.py   # Embedded font data
├── resources.py         # Bundled assets (icons, images)
├── settings.json        # Persistent user settings
├── requirements.txt      # Python dependencies
└── setup/               # InstallForge assets (scripts, images)
```

---

## Dependencies

| Package | Version | Purpose |
|---------|---------|---------|
| PyQt6 | 6.10.2 | UI framework & multimedia playback |
| PyInstaller | 6.19.0 | Packaging to standalone executable |
| clipboard | 0.0.4 | Clipboard utilities |

See [`requirements.txt`](requirements.txt) for the full list.

---

## Code Signing Policy

Free code signing for this open-source project is provided by **[SignPath.io](https://about.signpath.io)**, with the certificate issued by **[SignPath Foundation](https://signpath.org)**.

### What this means for you

When you download the Windows `.exe` from the official releases page, the binary is digitally signed. This signature verifies that:

- The binary was built from the source code in **this exact repository**
- The build process was automated and verifiable — no manual tampering
- The certificate is held by SignPath Foundation (not a personal cert), so you can trust the provenance

### Team roles

| Role | Responsibility | Members |
|------|----------------|---------|
| **Authors / Committers** | Trusted to commit directly to the repository | [@mahmedalam](https://github.com/mahmedalam) |
| **Reviewers** | Review pull requests from external contributors | [@mahmedalam](https://github.com/mahmedalam) |
| **Approvers** | Approve each signing request before a release is signed | [@mahmedalam](https://github.com/mahmedalam) |

> All team members use multi-factor authentication (MFA) on both GitHub and SignPath.

### Privacy policy

This program does **not** transfer any information to other networked systems unless specifically requested by the user or the person installing or operating it. YT Player has no telemetry, analytics, or network activity of any kind.

### Verifying a signature

On Windows, right-click the `.exe` → **Properties** → **Digital Signatures** tab. You should see a valid signature from **"SignPath Foundation"**.

---

## Contributing

Contributions are welcome! Here's how to get involved:

1. **Fork** the repository
2. **Create** a feature branch: `git checkout -b feature/your-feature`
3. **Commit** your changes: `git commit -m "Add your feature"`
4. **Push** to your branch: `git push origin feature/your-feature`
5. **Open a Pull Request** — a maintainer will review it

Please make sure your changes don't introduce any proprietary dependencies, and keep the code style consistent with the existing codebase.

---

## Reporting Issues

Found a bug or have a feature request? [Open an issue](https://github.com/mahmedalam/ytplayer/issues) on GitHub. Please include your OS, Python version, and steps to reproduce.

---

## Author

**Ahmed Alam** — [@mahmedalam](https://github.com/mahmedalam)

---

## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

*Built with ❤️ using Python & PyQt6*
