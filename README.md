

# 🎨 Advanced Artistic Filter App (Colab Ready)

Transform your images into stunning artwork with **8 different artistic styles** using OpenCV! This enhanced version offers a wide range of filters from cartoon effects to vintage looks, all runnable in **Google Colab** without local setup.



## 🌟 Key Features

### 🖌️ **8 Professional Artistic Filters**
1. **Cartoon** - Classic comic-style effect with smooth colors and bold edges
2. **Pencil Sketch** - Convert photos into realistic pencil drawings
3. **Watercolor** - Simulate beautiful watercolor paintings
4. **Oil Painting** - Digital oil painting effect with brush strokes
5. **Pop Art** - Vibrant, posterized look with bold outlines
6. **Enhanced HD** - Professional image enhancement and sharpening
7. **Vintage** - Nostalgic sepia tones with film grain
8. **Grayscale Art** - Artistic black & white conversion

### 🎛️ **Advanced Controls**
- Adjust **every parameter** for each filter
- Save your favorite settings as **custom presets**
- Real-time preview of changes
- High-quality output in JPG format

### ☁️ **Cloud Ready**
- 100% **Google Colab compatible** - runs in your browser
- No installation needed for Colab version
- Works with **any JPG/PNG image**

---

## 🚀 Quick Start

### Option 1: Run in Google Colab (Recommended)
1. Open **[Google Colab](https://colab.research.google.com)**
2. Upload the notebook or Python script
3. Run all cells - you'll be prompted to upload your image
4. Choose a filter and customize to your liking!

### Option 2: Local Installation
```bash
# Clone the repository
git clone https://github.com/<your-username>/artistic-filter-app.git
cd artistic-filter-app

# Install requirements
pip install -r requirements.txt

# Run the app
python artistic_filter_app.py
```

---

## 🎚️ Available Presets

The app comes with carefully tuned presets for each filter:

```json
{
  "soft_cartoon": {
    "filter": "cartoon",
    "params": {
      "bilateral_iters": 4,
      "bilateral_d": 9,
      "bilateral_sigmaColor": 75,
      "bilateral_sigmaSpace": 75,
      "median_ksize": 7,
      "use_canny": false,
      "edge_dilate": 1,
      "posterize_levels": 12
    }
  },
  "pencil_sketch": {
    "filter": "pencil_sketch",
    "params": {
      "invert": true,
      "blur_ksize": 21,
      "edge_ksize": 3
    }
  },
  "watercolor": {
    "filter": "watercolor",
    "params": {
      "bilateral_iter": 3,
      "bilateral_d": 9,
      "sigmaColor": 50,
      "sigmaSpace": 50,
      "median_ksize": 5
    }
  },
  "oil_painting": {
    "filter": "oil_painting",
    "params": {
      "size": 7,
      "dynRatio": 1
    }
  },
  "pop_art": {
    "filter": "pop_art",
    "params": {
      "num_colors": 8,
      "edge_thickness": 2
    }
  }
}
```

*(Additional presets included in the full app)*

---

## 🛠️ Technical Details

### 🔧 Dependencies
- Python 3.6+
- OpenCV (`opencv-python`)
- NumPy
- Matplotlib (for display)
- Google Colab `files` module (Colab version only)

Install locally with:
```bash
pip install opencv-python numpy matplotlib
```

### 🖼️ Supported Image Formats
- JPEG (.jpg, .jpeg)
- PNG (.png)

### 📁 Output
- Saves as high-quality JPG
- Preserves original image dimensions
- Side-by-side comparison with original

---

## 📜 License

This project is licensed under the **MIT License** - free for personal and commercial use.


4. Save your custom presets for frequently used styles

Enjoy creating stunning artistic versions of your photos! 🎨✨
