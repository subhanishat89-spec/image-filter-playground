# 🖼️ Image Filter Playground

A browser-based image processing tool built with vanilla HTML, CSS, and JavaScript. Every filter is implemented from scratch with pixel math and convolution kernels on the HTML5 Canvas. No libraries, no server, and no uploads: images never leave your device.

🔗 **Live Demo:** [subhanishat89-spec.github.io/image-filter-playground](https://subhanishat89-spec.github.io/image-filter-playground/)

![Screenshot](screenshot.png)

## ✨ Features

- 🎨 8 filters: Grayscale, Sepia, Invert, Threshold, Blur, Sharpen, Emboss, and Sobel edge detection
- 🎚️ Adjustments: brightness, contrast, saturation, and filter strength (blend with the original)
- 📊 Live luminance histogram
- 👀 Hold-to-compare with the original image
- 📥 Download the result as PNG
- 🖱️ Drag and drop or file picker, plus a built-in sample image
- 🔒 100% client-side, so your images stay private
- 🌙 Dark mode and a responsive layout

## 🧠 How It Works

Each frame follows a simple pipeline:

1. Read the original pixels with `getImageData`
2. Apply brightness, contrast, and saturation adjustments per pixel
3. Apply the selected filter: per-pixel mapping (grayscale, sepia, invert, threshold) or a 3×3 convolution (blur, sharpen, emboss), or Sobel gradients for edge detection
4. Blend the filtered result with the adjusted image using the strength slider
5. Draw the result with `putImageData` and update the histogram

## 🛠️ Tech Stack

HTML5 Canvas · CSS3 (custom properties, grid) · JavaScript (ES6+)

## 🚀 Run Locally

```bash
git clone https://github.com/subhanishat89-spec/image-filter-playground.git
cd image-filter-playground
```

Open `index.html` in your browser. No installation needed.

## 🔮 Future Improvements

- ↩️ Undo/redo history
- 🔀 Combine multiple filters in sequence
- 🎛️ Custom convolution kernel editor

## 👤 Author

**Nishat Subha** · [@subhanishat89-spec](https://github.com/subhanishat89-spec)
