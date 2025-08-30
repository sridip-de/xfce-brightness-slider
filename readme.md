**Draft:**
Here’s a clean `README.md` you can use on GitHub for your project.

````markdown
# Redshift Tray Controller

A simple **system tray utility** for Linux that lets you control screen **color temperature** and **brightness** using [Redshift](http://jonls.dk/redshift/).  
Built with Python, GTK3, and AppIndicator.

---

## Features

- 🖥️ Tray icon in system panel (no extra window unless opened).  
- 🎚️ Sliders to adjust:
  - **Color temperature** (1000K – 10000K).  
  - **Brightness** (0.1 – 1.0).  
- 🚀 Changes applied instantly via Redshift (`-P` mode).  
- 🛑 Clean quit option from tray menu.  
- 🎛️ Popup window stays hidden until you open it.

---

## Requirements

- Linux desktop environment with AppIndicator support (e.g., GNOME, XFCE, Cinnamon, etc.)  
- Python 3  
- Redshift  
- GTK3 and AppIndicator bindings for Python  

On Debian/Ubuntu/Mint:

```bash
sudo apt install redshift python3-gi gir1.2-appindicator3-0.1
````

On Fedora:

```bash
sudo dnf install redshift python3-gobject libappindicator-gtk3
```

---

## Installation

1. Clone this repository:

   ```bash
   git https://github.com/sridip-de/xfce-brightness-slider.git
   cd redshift-tray
   ```

2. Make script executable:

   ```bash
   chmod +x redshift.py
   ```

3. Run:

   ```bash
   ./redshift.py
   ```

---

## Usage

* The tray icon will appear in your system panel.
* Click the icon → **Controls** → adjust sliders.
* **Temperature** slider shifts the screen color.
* **Brightness** slider dims or brightens the display.
* **Quit** exits the tray app and resets Redshift settings.

---

## Notes

* The app uses `redshift -P -O <temp> -b <brightness>` internally.
* Ensure no other screen color/brightness manager conflicts with Redshift (e.g., Night Light, f.lux).
* Brightness is limited to safe values (0.1–1.0) to avoid hardware conflicts.

---

## License

MIT License – feel free to use, modify, and share.

```

---
