# Avarwand Picture Converter (APC)

A **fast, elegant, Python-based GUI tool** that converts modern and legacy image formats to **JPEG, PNG, BMP, WebP, or TIFF** – with **100% quality** and **zero hassle**.

**No command line. No quality loss. No complexity.**

---

## 🚀 Main Features

### Universal Format Support
Convert from **13 different image formats**:

**Standard Formats:**
- **HEIC/HEIF** → JPEG / PNG / BMP / WebP / TIFF
- **WebP** → JPEG / PNG / BMP / TIFF
- **AVIF** → JPEG / PNG / BMP / WebP / TIFF
- **JXL (JPEG XL)** → JPEG / PNG / BMP / WebP / TIFF
- **TIFF** → JPEG / PNG / BMP / WebP (with multi-page extraction)

**RAW Camera Formats:**
- **ARW** (Sony) → JPEG / PNG / BMP / WebP / TIFF
- **DNG** (Adobe) → JPEG / PNG / BMP / WebP / TIFF
- **ORF** (Olympus) → JPEG / PNG / BMP / WebP / TIFF
- **CR2** (Canon) → JPEG / PNG / BMP / WebP / TIFF

**HDR/Scientific Formats:**
- **EXR** (OpenEXR) → JPEG / PNG / BMP / WebP / TIFF
- **FITS** (Astronomy) → JPEG / PNG / BMP / WebP / TIFF

### Core Features
- ✨ **One-click batch conversion** – select 1 or 1000 files at once
- 🎯 **Maximum quality output** – Quality=100, no subsampling, no compression artifacts
- 📄 **Multi-page TIFF extraction** – Each page saved as separate file
- 🎨 **16-bit RAW processing** – Professional-grade color depth before conversion
- 🖥️ **Dark-mode UI** – Modern, clean interface with perfect alignment
- 📊 **Real-time progress** – Live status bar and file counter
- 🎭 **Custom icon** – Embedded base64 icon, no external files needed
- 📁 **Smart output** – Defaults to Desktop, easily customizable
- 🔧 **Auto-dependency installer** – Libraries installed automatically on first run
- 🪟 **Centered window** – 700×600 fixed size, auto-centers on screen

---

## 💎 Quality Settings

**Maximum quality for every format:**

| Output Format | Settings | Quality Level |
|--------------|----------|---------------|
| **JPEG** | Quality 100, no subsampling (4:4:4), optimize=False | 99.9% |
| **PNG** | compress_level=0 (no compression) | 100% |
| **WebP** | Quality 100, method 6 | 99.5% |
| **TIFF** | Adobe Deflate (lossless compression) | 100% |
| **BMP** | Uncompressed | 100% |

**RAW Processing:** 16-bit workflow → 8-bit conversion for maximum color fidelity

---

## 📋 System Requirements

### Minimum (Basic Formats)
- **OS**: Windows 10/11, Linux (Ubuntu 20.04+), macOS 10.15+
- **Python**: 3.8 or higher
- **RAM**: 2 GB
- **Dependencies**: `Pillow`, `pillow-heif`
- **Formats Available**: HEIC, HEIF, WebP, TIFF (4 formats)

### Recommended (All Formats)
- **OS**: Windows 10/11 (64-bit)
- **Python**: 3.9+
- **RAM**: 4 GB (8 GB for large RAW files)
- **Dependencies**: See [Installation](#installation) section
- **Formats Available**: All 13 formats

### Standalone Executable
- **No Python required** – Runs on any compatible Windows system
- **No installation** – Just download and run
- **All dependencies bundled** – 150-200 MB single file

---

### Option 2: Standalone Executable (Easiest)

1. Download `APC.exe` from [Releases](https://github.com/avarwand/APC/releases)
2. Run directly – no installation needed
3. All dependencies included

---

## 🎯 How to Use


### Converting Images

1. **Select Source Format** from dropdown (HEIC, WebP, AVIF, etc.)
2. Click **Browse** → select your image(s)
   - Multi-select supported (Ctrl+Click or Shift+Click)
   - Accepts any number of files
3. **Choose Output Format** (JPEG, PNG, BMP, WebP, TIFF)
4. **Set Output Path** (optional – defaults to Desktop)
5. Click **Start Conversion**
6. Watch the progress bar → **Done!**

### Special Features

**Multi-Page TIFF:**
- Automatically detects pages
- Saves each page as: `filename_page_1.png`, `filename_page_2.png`, etc.
- Single-page TIFFs saved normally

**RAW Files:**
- 16-bit processing with camera white balance
- Automatic brightness adjustment
- Professional color accuracy

---

## 🎨 User Interface

- **Window Size**: 700×600 pixels (fixed, non-resizable)
- **Position**: Auto-centers on screen
- **Color Scheme**: Dark mode (#2a2a2a background)
- **Font**: Segoe UI (Windows), system default (Linux/Mac)
- **Components**:
  - Source format dropdown
  - Output format dropdown
  - File browser with counter
  - Output path selector
  - Progress bar with percentage
  - Live status label
  - Info dialog with format details

---

## 📦 Available Formats

### Always Available (with Pillow)
✅ **WebP** input and output  
✅ **TIFF** input and output (multi-page support)

### Optional (Install as needed)

| Format | Library | Install Command |
|--------|---------|----------------|
| HEIC/HEIF | pillow-heif | `pip install pillow-heif` |
| AVIF | pillow-avif-plugin | `pip install pillow-avif-plugin` |
| JXL | pillow-jxl-plugin | `pip install pillow-jxl-plugin` |
| RAW (ARW, DNG, ORF, CR2) | rawpy | `pip install rawpy` |
| EXR | OpenEXR | `pip install OpenEXR` |
| FITS | astropy | `pip install astropy` |

**Note**: The app will show which formats are available based on installed libraries.

---

## 📊 Performance

| Operation | Speed | Notes |
|-----------|-------|-------|
| HEIC/WebP/AVIF | Fast | ~1-2 seconds per file |
| RAW formats | Moderate | ~5-10 seconds per file (CPU-intensive) |
| Multi-page TIFF | Fast | ~1 second per page |
| Large files (50MP+) | Moderate | Depends on RAM |
| Batch (100 files) | Automatic | Progress bar shows status |

**RAM Usage**: Approximately 200-500 MB per 24MP image during processing

---

## 🆘 Troubleshooting

### Format Not Available
**Problem**: Format missing from dropdown  
**Solution**: Install the required library (see table above)

### Conversion Fails
**Problem**: "Error converting file" message  
**Solution**: 
- Check file isn't corrupted
- Ensure enough disk space
- Try converting one file at a time

### Slow RAW Conversion
**Problem**: RAW files converting slowly  
**Solution**: This is normal – RAW processing is CPU-intensive

### Icon Not Showing
**Problem**: No icon in title bar  
**Solution**: Icon generation failed – app works normally, just no icon

### Executable Too Large
**Problem**: .exe is 200+ MB  
**Solution**: This is normal with all dependencies bundled

---

## License

**APC is freeware**, released under a custom End User License Agreement (EULA) by **Avarwand**.

In short, you are free to:

* **Use** APC free of charge, for both personal and commercial purposes
* **Share** APC with anyone, redistributing, hosting, mirroring, and promoting it is welcome, as long as it is passed on **complete and unmodified**, **free of charge**, and with clear credit to **Avarwand**

And you may not:

* Sell APC, monetize access to it, or lock it behind paywalls, donations, surveys, registration walls, or paid bundles
* Reverse engineer, decompile, or modify it (except to the limited extent permitted by applicable law)
* Claim it as your own work, or remove its copyright and branding notices

APC is provided **"as is"**, without warranty of any kind.

*This summary is for convenience only. The legally binding terms are in the [LICENSE](LICENSE.md) file included with every release and in this repository.*

---

**Developed by Avarwand**  
**Latest Version: February 2026**
**Initial Release: October 2025**  

---

## Contact

**Avarwand Support**  
📧 [avarwand@yahoo.com](mailto:avarwand@yahoo.com)  
🌐 [github.com/avarwand](https://github.com/avarwand/)

© 2025–2026 Avarwand. All rights reserved.

---
