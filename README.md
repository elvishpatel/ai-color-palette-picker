# 🎨 AI Personal Color Palette Picker

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-Open-green)](https://ai-color-platter.netlify.app/)

**AI Personal Color Palette Picker** is a privacy-first, intelligent web application that helps you discover your most flattering color palette based on your unique skin tone. Powered by modern AI and color science, everything runs 100% in your browser — your photos never leave your device!

![AI Color Palette Picker Screenshot](https://github.com/user-attachments/assets/9a59626a-93e4-4ebf-99db-e7f04a4e7272)

> **Privacy First:** All processing is done locally in your browser. No images are ever uploaded or stored anywhere.

---

## ✨ Features

- **100% Client-Side Processing**: Ensures absolute privacy—images never leave your device.
- **AI-Powered Face Detection**: Uses TensorFlow.js and BlazeFace to accurately sample skin from your portrait.
- **Personalized Palette Generation**: Creates a custom 8-color palette to suit your undertone and color season.
- **Advanced Skin Analysis**: Calculates average RGB/HEX/HSV, analyzes undertone & color season (Spring, Summer, Autumn, Winter).
- **Manual Adjustment**: Move or resize the sampling area for perfect accuracy.
- **Export & Share**: Copy your results as JSON or download your palette as a PNG image.
- **Fashion & Makeup Advice**: Get AI-generated style advice based on your analysis.

---

## 🚀 Live Demo

👉 [Try It Now!](https://ai-color-paletter.netlify.app/)

---

## 🛠️ How It Works

1. **Upload a clear, well-lit portrait photo.**
2. **AI detects your face and selects optimal skin areas** for sampling.
3. **Manual override:** Want more control? Adjust the sampling area manually!
4. **Skin pixels are analyzed** to find your average skin color.
5. **Your palette is crafted** with Colormind.io API and advanced color theory algorithms.
6. **Receive a detailed color profile & palette** with tailored fashion/makeup suggestions.

---

## 🖥️ Tech Stack

- **Frontend:** HTML5, CSS3, modern (ES6+) JavaScript — _no frameworks required_
- **AI:** `TensorFlow.js` + `BlazeFace` (on-device face detection)
- **Color Analysis:** Custom algorithms (RGB, HSV, YCbCr conversions, heuristic rules)
- **Palette Generation:** [Colormind.io API](http://colormind.io/) fallback to custom color theory logic if offline

---

## 💡 Usage

1. **Clone the repository:**
    ```bash
    git clone https://github.com/elvishpatel/ai-color-palette-picker.git
    cd ai-color-palette-picker
    ```
2. **Open `index.html` in any modern browser** (Chrome, Firefox, Edge, Safari).

### Using the App

1. Click “📷 Upload Image” and select a clear, front-facing photo.
2. Wait for face detection, or manually adjust the sampling area.
3. Click “✨ Analyze My Colours” to get your results.
4. Browse your custom palette, review advice, or export your palette as PNG/JSON.

---

## 📸 Screenshots

![App Screenshot](https://github.com/user-attachments/assets/9a59626a-93e4-4ebf-99db-e7f04a4e7272)
*AI analyzes your face for optimal color matching.*

---

## 🤝 Contributing

PRs, suggestions, and ideas are welcome!  
If you find bugs or want to propose features, please [open an issue](https://github.com/elvishpatel/ai-color-palette-picker/issues).

---

## 👨‍💻 Author

**Elvish Patel** – [GitHub](https://github.com/elvishpatel)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---
