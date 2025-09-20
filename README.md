# AI Personal Color Palette Picker

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

An intelligent, client-side web application to help you discover your personal color palette based on your skin tone. This tool uses AI to automatically detect facial landmarks for accurate sampling and generates a palette of flattering colors for clothing and design.

![AI Color Palette Picker Screenshot](https://github.com/user-attachments/assets/9a59626a-93e4-4ebf-99db-e7f04a4e7272)

> **Note:** This is a fully private tool. Your photos are processed directly in your browser and are never uploaded to any server.

---

## ✨ Features

-   📸 **100% Client-Side Processing:** Your images stay on your device, ensuring complete privacy.
-   🤖 **AI-Powered Face Detection:** Uses TensorFlow.js and the BlazeFace model to automatically find the best areas on the cheeks and forehead for skin tone sampling.
-   🎨 **Personalized Palette Generation:** Creates a custom 8-color palette designed to complement your unique skin tone.
-   🔬 **In-Depth Skin Analysis:** Determines your skin's average RGB/HEX/HSV values and provides a heuristic-based analysis of your **undertone** (Warm, Cool) and **color season** (e.g., Autumn, Winter).
-   🖱️ **Manual Override & Control:** Easily adjust the sampling area by dragging the circle or resizing it with the handle.
-   📤 **Easy Export Options:** Copy the entire results object as JSON or export your new palette as a convenient PNG image.

---
 Check Live Project Here : [Click Me](https://ai-color-platter.netlify.app/)
---

## 🛠️ How It Works & Tech Stack

The application follows a simple yet powerful pipeline:
1.  A user uploads an image.
2.  **BlazeFace** (a TensorFlow.js model) runs in the browser to detect the face and its primary landmarks (eyes, nose, ears).
3.  Custom algorithms use these landmarks to calculate the most reliable sampling points on the **forehead and both cheeks**.
4.  The pixels in these sample areas are read from the canvas. Outliers due to harsh lighting or shadows are filtered out using luminosity trimming.
5.  A robust **median color** is calculated to find the most accurate skin tone.
6.  This skin tone is sent to the **Colormind.io API** to generate a well-balanced initial palette. A custom, color-theory-based fallback is used if the API is unavailable.
7.  The palette is then fine-tuned based on the calculated **undertone and season** to produce the final flattering colors.

### **Technology Used:**
-   **Frontend:** Plain HTML5, CSS3, and modern JavaScript (ES6+). No frameworks.
-   **AI/Machine Learning:**
    -   **TensorFlow.js:** For running the machine learning model directly in the browser.
    -   **BlazeFace:** A lightweight, high-performance face detection model.
-   **Color Science:**
    -   Conversion functions for RGB, HSV, and YCbCr color spaces to analyze skin properties.
    -   Custom algorithms to determine undertone and adjust palettes based on color theory.
-   **API:**
    -   **Colormind.io API:** Used for initial palette generation.

---

## 🚀 Getting Started

This is a standalone project. No complex setup or build steps are required.

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/elvishpatel/ai-color-palette-picker.git
    ```
2.  **Navigate to the directory:**
    ```bash
    cd ai-color-palette-picker
    ```
3.  **Open the HTML file** (`index.html` or the project's main HTML file) in a modern web browser like Chrome, Firefox, or Edge.

### **Usage Guide**

1.  Click **"📷 Upload Image"** and select a clear, well-lit photo of yourself. Photos taken in natural daylight work best!
2.  The app will automatically detect your face and highlight the optimal sampling points.
3.  (Optional) If you need to make adjustments, click and drag the main circle to move it, or drag the handle on the right to resize it.
4.  Click **"✨ Analyze Skin Tone"** to process the image.
5.  View your detailed skin analysis and the suggested clothing color palette.
6.  Use the **"📋 Copy Palette JSON"** or **"⬇️ Export Palette PNG"** buttons to save your results.

---

## ✍️ Author

Developed with 💗 by **Elvish Patel**.

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.
