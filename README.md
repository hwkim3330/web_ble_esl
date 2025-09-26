# 🏷️ NEMR Electronic Shelf Label Web App

A modern web application for uploading images to NEMR Electronic Shelf Labels (ESL) using Web Bluetooth API.

![ESL Demo](https://img.shields.io/badge/Web%20Bluetooth-API-blue) ![GitHub Pages](https://img.shields.io/badge/GitHub-Pages-green)

## ✨ Features

### 🔍 NEMR Device Filtering
- Automatically filters and shows only Bluetooth devices with "NEMR" prefix
- Streamlined device selection process
- Real-time connection status with upload readiness check

### 📐 2.9" Landscape Optimisation
- Canvas locked to **296×128 px** (NEMR 2.9" resolution)
- Optional 180° flip for upside-down installations
- Pixel packing mirrors the official Arduino firmware (no red-wash issue)

### 🎨 Fabric.js Drawing Workspace
- Powered by Fabric.js for smooth, reliable editing
- Tools: brush, eraser, text, rectangle, circle, line
- Adjustable brush size (1–40 px) and colour picker
- Drag & drop or file picker image import with auto-fit scaling
- Quick actions: clear canvas, sample layout, PNG download

### 🌓 Modern UI/UX
- Dark/Light theme toggle with persistence
- Responsive layout for desktop and tablet
- Activity log with timestamped BLE protocol events

### 🔧 Technical Features
- Fully client-side – no server uploads needed
- **Complete ESL protocol implementation** (0x01/0x02/0x03 handshake + ACK retries)
- Accurate B/W + red plane packing (mirrored X columns) for NEMR tags
- Detailed logging of each command, ACK, and retry
- Web Bluetooth API integration (FEF0/FEF1/FEF2)

## 🚀 Live Demo

Visit the live application: **[https://hwkim3330.github.io/web_ble_esl/](https://hwkim3330.github.io/web_ble_esl/)**

## 🖥️ Browser Support

This application requires browsers with Web Bluetooth API support:
- ✅ Chrome/Chromium (Desktop & Mobile)
- ✅ Microsoft Edge
- ❌ Firefox (limited support)
- ❌ Safari (not supported)

## 📋 Usage Instructions (2.9" ESL)

1. **Connect** – Click "Connect to NEMR Device" (only NEMR-prefixed devices are shown).
2. **Design** – Draw with the brush, add shapes/text, or import an image (auto scaled to 296×128).
3. **Orientation** – Leave at `Landscape (0°)` for normal mounting. Use `Flip 180°` if the tag is upside-down.
4. **Review** – Optional: download PNG or drop in the included sample layout for testing.
5. **Upload** – Click "Upload to ESL" to run the BLE handshake and transfer (progress + ACK logs shown).

> ⚠️ 90°/270° portrait rotation is not supported on NEMR 2.9" hardware because the panel firmware expects 296 columns. Use the 180° flip if the device is installed upside-down.

## 🏷️ NEMR Device Filter

The Bluetooth device selector is configured to show only devices with names starting with "NEMR", ensuring you connect to the correct ESL devices.

## 📁 Project Structure

```
web_ble_esl/
├── index.html          # Main application file
├── .github/workflows/  # GitHub Actions for Pages deployment
└── README.md           # This file
```

## 🤝 Contributing

Based on the excellent work by [atc1441](https://github.com/atc1441/ATC_GICISKY_ESL) and inspired by [shelflabels.andrewgraham.dev](https://shelflabels.andrewgraham.dev/).

## ⚠️ Disclaimer

This tool is provided as-is for educational and development purposes. Use at your own risk with compatible ESL devices.

## 📄 License

MIT License - feel free to modify and distribute.

---

Made with ❤️ for the ESL development community
