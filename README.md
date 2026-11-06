# 🖼️ BulkCollaze — High-Performance Batch Collage Maker & PDF Extractor (PWA)

**BulkCollaze** is an ultra-fast, privacy-first, progressive web application (PWA) designed to instantly group multiple photos and PDF pages into high-resolution, uniform grid collages.

Built entirely with modern vanilla JavaScript and lightweight HTML5 Canvas, all image processing happens **100% locally inside the browser**. No files are ever uploaded to external servers.

---

## ✨ Features

* **📱 Progressive Web App (PWA):** Can be installed on Desktop, Android, and iOS. Works 100% offline via Service Workers.
* **📄 PDF Support:** Drag & drop multi-page PDF documents to extract pages directly into photo collage grids.
* **⚡ Equal Cell Grid Engine:** Extra images on the final collage page maintain the exact same cell dimensions as preceding pages.
* **📐 Custom Aspect Ratios & Presets:**
  * **Aspect Ratios:** A4 Print (Default), 1:1 Square, 4:5 Instagram, 9:16 Mobile Story, and 16:9 Widescreen.
  * **Photos Per Page:** Presets for `1, 2, 3, 4, 6, 8, 9, 12` photos per page.
* **🎨 Custom Borders & Spacing:**
  * Toggleable Photo Borders (Solid, Dashed, Dotted, or None) with customizable width, color, and inner photo padding.
  * Adjust photo spacing (up to 180px), page margins, corner radius, and image box height scaling.
* **🔍 Fit & Auto-Rotate Modes:** Choose between **Contain (100% No Crop)** and **Cover (Fill Cell)** with intelligent auto-rotation matching cell orientation.
* **📦 Multiple Export Formats:** Export collages as high-quality **JPG**, crisp **PNG**, or compiled **Multi-Page PDF** documents, with optional single-click **ZIP batch export**.

---

## 🛠️ Tech Stack & Dependencies

* **HTML5 / Canvas API:** High-resolution multi-tier grid rendering engine.
* **Tailwind CSS (CDN):** Modern, lightweight Google Material Lite interface styling.
* **JSZip & FileSaver.js:** Client-side ZIP generation for bulk downloads.
* **jsPDF:** Dynamic multi-page PDF document creation.
* **PDF.js:** High-fidelity in-browser rendering of uploaded PDF documents.

---

## 🚀 Quick Start / Local Deployment

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/YOUR_USERNAME/bulkcollaze.git
   cd bulkcollaze
   ```

2. **Run Locally:**
   Simply open `index.html` in any web browser!

3. **Deploy to GitHub Pages:**
   * Go to **Repository Settings > Pages**.
   * Select `Deploy from a branch` -> `main` / `/ (root)`.
   * Save and visit your live HTTPS link!

---

## 📂 Project Hierarchy

```
bulkcollaze/
├── index.html        # Main App Interface & Canvas Engine
├── manifest.json     # PWA Configuration & Metadata
├── sw.js             # Service Worker for Offline Caching
├── icon-192.png      # 192x192 App Icon
├── icon-512.png      # 512x512 App Icon
└── README.md         # Project Documentation
```

---

## 🔒 Privacy & Security

All image rendering, PDF parsing, grid calculations, and file zip operations occur locally on your machine using client-side Web APIs. **Zero telemetry, zero image uploads.**

---

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.
