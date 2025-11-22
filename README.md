# Chojema Image AutoTrimmer

Chojema Image AutoTrimmer is a browser-based tool that automatically trims excess background from an image so it tightly fits the main object. It runs entirely client-side, allowing quick previews and downloads without uploads or installs.

## Features
- Drag-and-drop or file picker upload for common image formats (PNG, JPG, etc.).
- Automatic detection of non-background pixels to crop around the subject.
- Adjustable margin padding and background tolerance to fine-tune results.
- Side-by-side original and trimmed canvas previews with dimensions.
- One-click download of the cropped image with timestamped filenames.
- Korean and English UI toggle.

## Usage
1. Open `index.html` in a modern browser.
2. Select or drop an image into the upload area.
3. Optionally adjust **Margin (px)** to retain some border and **Background tolerance** to handle noisy edges.
4. Click **Run auto trim** to crop the image.
5. Review the **Result image** preview and click **Download result image** to save the trimmed PNG.

## Controls
- **Margin (px):** Adds padding around the detected bounds (0–200 px).
- **Background tolerance:** Loosens or tightens how similar a pixel can be to the background before being kept (5–100).
- **Language:** Switch between 한국어 and English from the top-right buttons.

## Output
The downloaded file uses the original filename with a timestamp suffix (e.g., `photo-2025-11-13_19-50-43.png`). If no non-background pixels are found, the original image is preserved.

## License
MIT
