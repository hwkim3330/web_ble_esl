# 🏷️ NEMR Electronic Shelf Label Web App

A modern web application for uploading images to NEMR Electronic Shelf Labels (ESL) using Web Bluetooth API.

![ESL Demo](https://img.shields.io/badge/Web%20Bluetooth-API-blue) ![GitHub Pages](https://img.shields.io/badge/GitHub-Pages-green)

## ✨ Features

### 🔍 NEMR Device Filtering
- Automatically filters and shows only Bluetooth devices with "NEMR" prefix
- Streamlined device selection process
- Enhanced user experience for NEMR ESL devices

### 🔄 Default Rotation Support
- **90° rotation applied by default** for optimal ESL display orientation
- Additional rotation controls: 90°, 180°, 270°
- Smart canvas resizing based on rotation angle

### 🎨 Drawing & Upload Tools
- **Interactive drawing canvas** with brush tools
- Color picker and adjustable brush size
- Drag & drop image upload support
- Canvas clearing and view/draw mode toggle

### 🌓 Modern UI/UX
- Dark/Light theme toggle with persistence
- Mobile-responsive design
- Card-based layout with smooth animations
- Real-time connection status indicators

### 📱 Device Compatibility
- Supports multiple ESL display sizes:
  - 296x128 (2.9")
  - 200x200 (1.54")
  - 250x122 (2.13")
  - 400x300 (4.2")

### 🔧 Technical Features
- **Client-side processing** - no server uploads
- Web Bluetooth API integration
- Image to bitmap conversion
- Touch support for mobile devices
- Progressive Web App ready

## 🚀 Live Demo

Visit the live application: **[https://hwkim3330.github.io/web_ble_esl/](https://hwkim3330.github.io/web_ble_esl/)**

## 🖥️ Browser Support

This application requires browsers with Web Bluetooth API support:
- ✅ Chrome/Chromium (Desktop & Mobile)
- ✅ Microsoft Edge
- ❌ Firefox (limited support)
- ❌ Safari (not supported)

## 📋 Usage Instructions

1. **Connect Device**: Click "Connect to NEMR Device" to scan for NEMR-labeled Bluetooth devices
2. **Select Display Size**: Choose your ESL device's display dimensions
3. **Upload/Draw Image**:
   - Drag & drop an image file, or
   - Click the upload area to select a file, or
   - Toggle drawing mode and create custom graphics
4. **Apply Rotation**: Use rotation controls as needed (90° applied by default)
5. **Upload to Device**: Click "Upload to ESL Device" to send the image

## 🔄 Default Rotation

The application automatically applies a **90° rotation** when the page loads, optimized for typical ESL mounting orientations. You can adjust this using the rotation controls.

## 🎨 Drawing Features

- **Drawing Mode**: Toggle between view and drawing modes
- **Color Picker**: Select any color for drawing
- **Brush Size**: Adjustable from 1-20 pixels
- **Clear Canvas**: Reset the canvas to white background

## 🏷️ NEMR Device Filter

The Bluetooth device selector is configured to show only devices with names starting with "NEMR", ensuring you connect to the correct ESL devices.

## 📁 Project Structure

```
web_ble_esl/
├── index.html          # Main application file
├── .github/workflows/  # GitHub Actions for Pages deployment
└── README.md          # This file
```

## 🤝 Contributing

Based on the excellent work by [atc1441](https://github.com/atc1441/ATC_GICISKY_ESL) and inspired by [shelflabels.andrewgraham.dev](https://shelflabels.andrewgraham.dev/).

## ⚠️ Disclaimer

This tool is provided as-is for educational and development purposes. Use at your own risk with compatible ESL devices.

## 📄 License

MIT License - feel free to modify and distribute.

---

Made with ❤️ for the ESL development community