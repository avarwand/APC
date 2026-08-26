# Avarwand Picture Converter (APC)
A **powerful, modern GUI tool** for **batch converting pictures** between 15 input and 5 output formats, and for **compressing pictures to a target file size**, with precision, speed, and safety.

No command line . No risk . Full control

---

## What's New in v2.3
- **Import rectangle**: click to browse, or simply **drag & drop** your pictures into the app
- **Mixed-format import**: bring JPEGs, PNGs, RAW shots and more in together — every file is recognized automatically
- **JPEG, PNG and BMP** now accepted as input formats (**15 input formats** in total)
- **Imported-files list**: every picture listed with its complete name — select one, several, or all and take them out (**Remove selected** / **Clear input**)
- **Compression Mode**: shrink same-format pictures to a chosen maximum file size with the new **target-size slider**
- Conversion always at the **best possible quality** of the target format, transparency preserved
- Redesigned, scrollable **Info window**

---

## Main Features
- **Batch convert pictures** between formats in one operation  
- **15 input formats**: standard, RAW camera, and HDR/scientific pictures  
- **5 output formats**: JPEG, PNG, BMP, WebP, TIFF  
- **Import by click or drag & drop**, any mix of formats at once  
- **Automatic format recognition** for every single file  
- **File list with multi-select removal**: full control over what gets processed  
- **Compression Mode**: reduce pictures to a maximum file size, at the best quality that fits  
- **Best possible quality, always**: lossless where the format allows it, transparency preserved  
- **Multi-page TIFF**: every page saved as its own picture  
- **16-bit RAW processing** for maximum quality  
- **Background processing** with progress bar: the window never freezes  
- **Dark-mode GUI** with clean layout  
- **Fully GUI-based**: no CLI knowledge required  
- **Works on large batches** with hundreds of pictures  

---

## Input Formats (15)

- **Standard**: JPEG, PNG, BMP, WebP, TIFF, HEIC, HEIF, AVIF, JXL
- **RAW Camera**: ARW, DNG, ORF, CR2
- **HDR / Scientific**: EXR, FITS

All accepted formats are shown directly on the import rectangle, and any mix of them can be imported together.

---

## Output Formats & Quality

Conversion always uses the highest possible quality of the target format:

- **JPEG**: Quality 100, no chroma subsampling (4:4:4)
- **PNG**: Lossless, transparency preserved
- **WebP**: Lossless, transparency preserved
- **TIFF**: Lossless Adobe Deflate compression
- **BMP**: Uncompressed (transparency flattened on white)

Multi-page TIFF inputs are split automatically: every page becomes its own file. RAW camera pictures are developed with 16-bit processing before saving.

---

## Compression Mode

Shrink pictures to a maximum file size **without changing their format**:

- Activates automatically when **all imported pictures already have the chosen output format**: *Start Conversion* switches off, **Start Compression** and the **size slider** switch on
- The **slider sets the maximum file size per picture**: its range runs from the smallest reachable size of the biggest imported picture up to its current size
- APC automatically finds the **best quality that still fits the target** for every single picture
- Format-specific compression: **JPEG / WebP** by quality search, **TIFF** by JPEG-in-TIFF, **PNG** by color reduction, **BMP** by bit-depth reduction
- Results are saved with a **"_compressed"** suffix: **your originals stay untouched**
- Pictures already below the target are copied unchanged; pictures that cannot reach the target are saved at their minimum possible size — the summary after the run reports both

---

## How to Use

1. Download the desired Version
2. Unzip it > Install it (_for the installer version_)
3. **Import pictures**: click the import rectangle or drag & drop files onto it — mixed formats welcome
4. Fine-tune the list if needed: **Remove selected** entries or **Clear input**
5. Choose the **Output Format** and the **Output Path**
6. Click **Start Conversion** — or, if all pictures already have the output format, set the **size slider** and click **Start Compression**
7. Watch the progress → **Done!**

---

## Safety Notes

* Conversion and compression **never modify or delete your originals**: new files are always written to the output folder
* Compressed pictures get a **"_compressed"** suffix, so nothing is ever overwritten
* Unsupported files are **skipped and reported**, never touched
* A **summary after every run** tells you exactly what was converted, compressed, copied unchanged, or saved at minimum size
* Designed to minimize accidental changes

---

## Use Cases

* Converting phone photos (HEIC / HEIF) for maximum compatibility
* **Shrinking pictures under email or upload size limits**
* Preparing web images: small files at the best quality that fits
* Developing RAW camera shots (ARW, DNG, ORF, CR2) into JPEG or TIFF
* Converting astro (FITS) and HDR (EXR) images into standard formats
* **Splitting multi-page TIFF scans into single pictures**
* Normalizing mixed picture libraries into one format
* Archiving pictures in lossless formats

---

## System Requirements
- **OS**: Windows 10 / Windows 11  

No external dependencies required.

---

## Contributing

This project is released as **freeware**.

While primarily maintained by the author, suggestions, bug reports, and improvement ideas are welcome via email.

Pull requests are currently not accepted.

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
**Latest Version: August 2026**
**Initial Release: October 2025**  

---

## Contact

**Avarwand Support**  
📧 [avarwand@yahoo.com](mailto:avarwand@yahoo.com)  
🌐 [github.com/avarwand](https://github.com/avarwand/)

© 2025–2026 Avarwand. All rights reserved.

---
