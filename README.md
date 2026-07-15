# XC Bodycam Configurator & Overlay

A premium, modern, and highly customizable HUD overlay for police and emergency services roleplaying. Designed for streaming and recording layouts, it is fully compatible with OBS Studio and other broadcasting software.

---

## Key Features

* **Premium UI/UX**: Modern dark glassmorphic design featuring glowing accents and responsive layouts.
* **Bilingual Toggle**: Switch between **English** and **Bahasa Indonesia** with a single click.
* **Visual Presets Grid**: Choose badges/logos instantly from a grid of presets (Axon, LSPD, LSSD) or input a custom image URL.
* **Logo Resizing**: Adjust the height of the badge on the overlay dynamically from 60px to 180px using a range slider.
* **Custom Rank & Name**: Prepend custom officer ranks (e.g. `Sgt.`, `Det.`) next to your name.
* **Real-time Clock**: Automatically parses dates and local times with timezone offsets using Moment.js.
* **Transparent HUD**: Perfect for overlays, featuring clean outlines and drop-shadows for high readability over gameplay.

---

## OBS Integration Guide

Follow these steps to overlay the real-time bodycam HUD onto your stream or recording:

1. Open the configurator (`index.html`) in your browser.
2. Customize your details (Officer Name, Callsign, Agency, Badge size/preset, etc.).
3. Click the **Copy Link** button.
4. Open OBS Studio:
   * In **Sources**, click **+** and choose **Browser**.
   * Name the source (e.g., *"Bodycam Overlay"*).
   * Paste the copied URL into the **URL** field.
   * Set **Width** to `500` and **Height** to `160`.
   * Click **OK**.
5. Position the source in the upper-right or upper-left corner of your stream canvas.

---

## Local Hosting Recommendation

If you prefer to run the overlay locally rather than hosting it on a remote web server:
1. Open a terminal in the project directory.
2. Serve the directory using Python:
   ```bash
   python -m http.server 8000
   ```
3. Open `http://localhost:8000/index.html` in your browser.
4. Generate the URL, copy the link, and paste it into OBS. This bypasses browser security restrictions on the `file://` protocol.

---

## Support the Developer

If you like this project and want to support its development:
* Donate via [Bagi Bagi](https://bagibagi.co/xppaicyberr)
* Send crypto to: `0xE11018C82D4405bDBc7414eC988Fd08351666666` (Base Chain)
