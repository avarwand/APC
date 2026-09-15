<div align="center">

# Avarwand Picture Converter 2.5.0

</div>

A **powerful, modern GUI tool** for **batch converting pictures** between 20 input and 7 output formats, and for **compressing pictures to a target file size**, with precision, speed, and safety.

> _No command line | No risk | Full control_

---

## What's New in v2.5
- **TGA and DDS** join as input **and** output formats (**20 input / 7 output formats** in total)
- **TGA**: read and written **losslessly** (RLE) with a full alpha channel, the classic game-pipeline format
- **DDS**: all common **DXT/BC texture variants** are read; written **uncompressed at maximum quality**
- **Import whole folders**: drop one or many folders, they are **searched to any depth**, and every supported picture inside is imported; only files are ever listed, never folders
- **Nothing gets overwritten anymore**: if two results would share a name (easy with nested folders), APC appends **_2, _3, ...** automatically
- **Compression Mode** covers the new formats too: **TGA** by RLE + color reduction, **DDS** by block compression (uncompressed → DXT5 → DXT1)
- **WebP lossless is now exact**: even the invisible colors under fully transparent pixels are preserved, game engines sample them

---

## Main Features
- **Batch convert pictures** between formats in one operation  
- **20 input formats**: standard, RAW camera, HDR/scientific, and game-texture pictures  
- **7 output formats**: JPEG, PNG, BMP, WebP, TIFF, TGA, DDS  
- **Import by click or drag & drop**, any mix of formats at once  
- **Whole folders welcome**: dropped folders are searched to any depth, only the pictures inside are listed  
- **Automatic format recognition** for every single file  
- **File list with multi-select removal**: full control over what gets processed  
- **Per-format counters** above the list: one click selects every picture of that format (Ctrl-click adds to the selection)  
- **Skipped files reported with their format** as gray counters, e.g. *XXX (skipped)*  
- **No output is ever overwritten**: a taken name automatically becomes *name_2*, *name_3*, ...  
- **Compression Mode**: reduce pictures to a maximum file size, at the best quality that fits  
- **Best possible quality, always**: lossless where the format allows it, transparency preserved  
- **Multi-page TIFF**: every page saved as its own picture  
- **16-bit RAW processing** for maximum quality  
- **Background processing** with progress bar: the window never freezes  
- **Dark-mode GUI** with clean layout  
- **Fully GUI-based**: no CLI knowledge required  
- **Works on large batches** with hundreds of pictures  

---

## Input Formats (20)

- **Standard**: JPEG, JFIF, PNG, BMP, WebP, TIFF, HEIC, HEIF, AVIF, JXL
- **RAW Camera**: ARW, CR2, CR3, DNG, NEF, ORF
- **HDR / Scientific**: EXR, FITS
- **Game / Texture**: DDS, TGA

All accepted formats are shown directly on the import rectangle, and any mix of them can be imported together.

---

## Output Formats & Quality

Conversion always uses the highest possible quality of the target format:

- **JPEG**: Quality 100, no chroma subsampling (4:4:4)
- **PNG**: Lossless, transparency preserved
- **WebP**: Lossless, transparency preserved (exact, even colors under fully transparent pixels are kept)
- **TIFF**: Lossless Adobe Deflate compression
- **BMP**: Uncompressed (transparency flattened on white)
- **TGA**: Lossless RLE compression, transparency preserved
- **DDS**: Uncompressed at maximum quality (no mipmaps, for final game textures use a dedicated texture tool)

Multi-page TIFF inputs are split automatically: every page becomes its own file. RAW camera pictures are developed with 16-bit processing before saving.

---

## Compression Mode

Shrink pictures to a maximum file size **without changing their format**:

- Activates automatically when **all imported pictures already have the chosen output format**: *Start Conversion* switches off, **Start Compression** and the **size slider** switch on
- The **slider sets the maximum file size per picture**: its range runs from the smallest reachable size of the biggest imported picture up to its current size
- APC automatically finds the **best quality that still fits the target** for every single picture
- Format-specific compression: **JPEG / WebP** by quality search, **TIFF** by JPEG-in-TIFF, **PNG** by color reduction, **BMP** by bit-depth reduction
- **JFIF pictures count as JPEG here**: with JPEG as output they enter Compression Mode and use the JPEG engine
- **TGA**: RLE + color reduction, **DDS**: uncompressed → DXT5 → DXT1
- Results are saved with a **"_compressed"** suffix: **your originals stay untouched**
- Pictures already below the target are copied unchanged; pictures that cannot reach the target are saved at their minimum possible size, the summary after the run reports both

---

## How to Use

1. Download the desired Version
2. Unzip it > Install it (_for the installer version_)
3. **Import pictures**: click the import rectangle or drag & drop files **or whole folders** onto it, mixed formats welcome, nested folders are searched completely
4. Fine-tune the list if needed: click a **format counter** to select a whole format, then **Remove selected**, or **Clear input**
5. Choose the **Output Format** and the **Output Path**
6. Click **Start Conversion**, or, if all pictures already have the output format, set the **size slider** and click **Start Compression**
7. Watch the progress → **Done!**

---

## Safety Notes

* Conversion and compression **never modify or delete your originals**: new files are always written to the output folder
* Compressed pictures get a **"_compressed"** suffix
* **Nothing is ever overwritten**: if an output name is already taken, APC appends *_2, _3, ...* automatically
* Unsupported files are **skipped and reported with their format**, never touched
* A **summary after every run** tells you exactly what was converted, compressed, copied unchanged, or saved at minimum size
* Designed to minimize accidental changes

---

## Use Cases

* Converting phone photos (HEIC / HEIF) for maximum compatibility
* **Shrinking pictures under email or upload size limits**
* Preparing web images: small files at the best quality that fits
* Developing RAW camera shots (Sony ARW, Canon CR2/CR3, Adobe DNG, Nikon NEF, Olympus ORF) into JPEG or TIFF
* Converting astro (FITS) and HDR (EXR) images into standard formats
* **Extracting game textures**: DDS files → PNG with transparency, ready to view and edit
* Writing TGA textures for game-engine and 3D pipelines
* **Converting a whole nested picture folder in one drop**
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
**Latest Version: September 2026**
**Initial Release: October 2025**  

---

## Contact

**Avarwand Support**  
📧 [avarwand@yahoo.com](mailto:avarwand@yahoo.com)  
🌐 [github.com/avarwand](https://github.com/avarwand/)

© 2025–2026 Avarwand. All rights reserved.

---
