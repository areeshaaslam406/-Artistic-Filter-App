
# 🎭 Artistic Filter App (Colab Ready)

Transform your images into artistic "cartoon-style" artwork using OpenCV and Python!  
This project allows you to apply **smooth color effects**, **edge detection**, and **posterization** to create stylized images.  
Run directly in **Google Colab** without local setup.

---

## 📌 Features
- 🎨 **Multiple Artistic Presets**
  - `soft_cartoon` → Smooth & subtle effect.
  - `strong_cartoon` → Bold, saturated cartoon style.
  - `sketchy` → Pencil-sketch style with Canny edges.
- ⚙️ **Custom Parameter Mode**
  - Fine-tune bilateral filtering, edge detection, posterization levels.
  - Save your favorite settings as **custom presets**.
- 💾 Save output as a high-quality `.jpg`.
- 🌐 100% **Google Colab ready** — works without installing dependencies locally.


## 🚀 Getting Started

### 1️⃣ Run in Google Colab
1. Open **Google Colab**: [https://colab.research.google.com](https://colab.research.google.com)
2. Upload `artistic_filter_app.py` to Colab.
3. Run all cells — you will be prompted to upload your image.

### 2️⃣ Local Installation (Optional)
```bash
# Clone repository
git clone https://github.com/<your-username>/artistic-filter-app.git
cd artistic-filter-app

# Install dependencies
pip install -r requirements.txt

# Run script
python artistic_filter_app.py
````

---

## ⚙️ Usage

When running the app:

1. **Upload** an image (JPG/PNG).
2. Choose a **preset** or type `"custom"` to enter your own parameters.
3. Optionally save your parameters as a **named preset**.
4. View and **download** the cartoonized result.

**Presets Included:**

```json
{
  "soft_cartoon": {
    "bilateral_iters": 4,
    "bilateral_d": 9,
    "bilateral_sigmaColor": 75,
    "bilateral_sigmaSpace": 75,
    "median_ksize": 7,
    "use_canny": false,
    "edge_dilate": 1,
    "posterize_levels": 12
  },
  "strong_cartoon": {
    "bilateral_iters": 7,
    "bilateral_d": 9,
    "bilateral_sigmaColor": 100,
    "bilateral_sigmaSpace": 100,
    "median_ksize": 7,
    "use_canny": false,
    "edge_dilate": 2,
    "posterize_levels": 8
  },
  "sketchy": {
    "bilateral_iters": 1,
    "bilateral_d": 9,
    "bilateral_sigmaColor": 50,
    "bilateral_sigmaSpace": 50,
    "median_ksize": 5,
    "use_canny": true,
    "canny_thr1": 50,
    "canny_thr2": 150,
    "edge_dilate": 1,
    "posterize_levels": null
  }
}


## 📦 Dependencies

* Python 3.x
* [OpenCV](https://opencv.org/) (`cv2`)
* NumPy
* Matplotlib
* Google Colab's `files` module (if running in Colab)

Install locally via:


pip install opencv-python numpy matplotlib


## 📜 License

This project is licensed under the **MIT License** — feel free to use, modify, and share.


