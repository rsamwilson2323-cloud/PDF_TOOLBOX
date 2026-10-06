# 📄 PDF Toolbox

> **A simple, modern, browser-based PDF utility toolbox for everyday PDF tasks.**

PDF Toolbox is a lightweight web application that brings common PDF operations into one clean interface. Select a task, choose your files using the visual upload area, and download the result directly from your browser.

**No Python installation. No command prompt. No complicated setup.**

---

## ✨ Features

- 📑 **Merge PDFs**
- ✂️ **Split PDF**
- 📄 **Extract Pages**
- 🗜️ **Optimize / Compress PDF**
- 🖼️ **Images → PDF**
- 📸 **PDF → Images**
- 💧 **Add Watermark**
- 📂 **Click-to-select file upload**
- 🖱️ **Drag-and-drop file selection**
- 📦 **ZIP download for multiple generated files**
- 🎨 **Modern dark purple glass-style UI**
- 📱 **Responsive interface**
- ⚡ **Browser-based processing**
- 🔒 **No project-specific cloud upload**
- 🚀 **Simple Chrome launcher**

---

# 🖥️ User Interface

The toolbox uses a task-based interface so you can choose exactly what you want to do.

```text
┌─────────────────────────────────────────────────────┐
│                                                     │
│                  📄 PDF TOOLBOX                     │
│                                                     │
│   ┌──────────────┐    ┌──────────────┐             │
│   │ 📑           │    │ ✂️           │             │
│   │ Merge PDFs   │    │ Split PDF    │             │
│   └──────────────┘    └──────────────┘             │
│                                                     │
│   ┌──────────────┐    ┌──────────────┐             │
│   │ 📄           │    │ 🗜️           │             │
│   │ Extract      │    │ Compress     │             │
│   └──────────────┘    └──────────────┘             │
│                                                     │
│   ┌──────────────┐    ┌──────────────┐             │
│   │ 🖼️           │    │ 📸           │             │
│   │ Images → PDF │    │ PDF → Images │             │
│   └──────────────┘    └──────────────┘             │
│                                                     │
│   ┌──────────────┐    ┌──────────────┐             │
│   │ 💧           │    │ 🔐           │             │
│   │ Watermark    │    │ Protect PDF  │             │
│   └──────────────┘    └──────────────┘             │
│                                                     │
└─────────────────────────────────────────────────────┘
```

---

# 🚀 Quick Start

## 1. Download the Project

Clone the repository:

```bash
git clone https://github.com/rsamwilson2323-cloud/PDF_TOOLBOX.git
```

Enter the project:

```bash
cd PDF_TOOLBOX
```

---

## 2. Open PDF Toolbox

You can simply open:

```text
PDF_TOOLBOX.html
```

in Google Chrome or another modern browser.

If the project includes the launcher:

```text
OPEN_PDF_TOOLBOX.bat
```

double-click it to open the toolbox in your default browser.

---

# 📄 Available Tools

## 1. 📑 Merge PDFs

Combine multiple PDF documents into a single PDF.

### Workflow

```text
Select Merge PDFs
        ↓
Choose multiple PDF files
        ↓
Merge & Download
        ↓
merged.pdf
```

---

## 2. ✂️ Split PDF

Split every page of a PDF into separate PDF files.

The generated files are packaged into a ZIP file for convenient downloading.

Example:

```text
input.pdf
   ↓
split-pages.zip
   ├── page-1.pdf
   ├── page-2.pdf
   ├── page-3.pdf
   └── ...
```

---

## 3. 📄 Extract Pages

Extract specific pages from a PDF.

Supported formats include:

```text
1,3,5
```

```text
1-5
```

```text
1,3,5-10
```

Example:

```text
Original PDF
    ↓
Pages: 1,3,5-8
    ↓
extracted-pages.pdf
```

---

## 4. 🗜️ Compress / Optimize PDF

Creates an optimized copy of the selected PDF using browser-side PDF optimization.

> **Note:** PDF compression results depend on the original document. A browser-side optimization pass cannot guarantee that every PDF will become smaller.

---

## 5. 🖼️ Images → PDF

Convert images into a PDF document.

Supported browser image formats include common formats such as:

```text
JPG
JPEG
PNG
```

Multiple images can be selected and combined into one PDF.

Example:

```text
photo1.jpg
photo2.jpg
photo3.png
      ↓
images.pdf
```

---

## 6. 📸 PDF → Images

Render PDF pages into PNG images.

The generated images are packaged into a ZIP file:

```text
pdf-images.zip
   ├── page-1.png
   ├── page-2.png
   ├── page-3.png
   └── ...
```

---

## 7. 💧 Add Watermark

Add a text watermark to every page of a PDF.

Example:

```text
CONFIDENTIAL
```

The watermark is placed diagonally across the page with transparency.

---

## 8. 🔐 Protect PDF

The Protect PDF card is included in the interface, but **true password-based PDF encryption is not enabled in the current browser-only build**.

For secure PDF encryption, use a dedicated PDF application or add a server/native PDF encryption engine to a future version.

---

# 📂 File Selection

PDF Toolbox provides a clean visual upload interface.

You can:

```text
Click to choose files
        OR
Drag and drop files
```

Selected files are displayed in an aligned list:

```text
┌─────────────────────────────────────────────┐
│ 📄 document-one.pdf                  2.4 MB │
│ 📄 document-two.pdf                  1.8 MB │
│ 📄 document-three.pdf                4.1 MB │
└─────────────────────────────────────────────┘
```

---

# 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| 🌐 HTML5 | Application structure |
| 🎨 CSS3 | UI and responsive design |
| ⚡ JavaScript | Application logic |
| 📄 PDF-LIB | PDF creation and manipulation |
| 📸 PDF.js | PDF rendering |
| 📦 JSZip | ZIP generation |
| 🌍 Browser APIs | File selection and downloads |

---

# 📦 Project Structure

```text
PDF_TOOLBOX/
│
├── 📄 PDF_TOOLBOX.html
│
├── 📄 OPEN_PDF_TOOLBOX.bat
│
├── 📄 README.md
│
└── 📄 LICENSE
```

### `PDF_TOOLBOX.html`

The main web application containing:

- User interface
- PDF operations
- File selection
- Drag-and-drop handling
- Download functionality

### `OPEN_PDF_TOOLBOX.bat`

Optional Windows launcher that opens the HTML application in the default browser.

### `README.md`

Project documentation.

### `LICENSE`

Project license.

---

# 🔐 Privacy

PDF Toolbox is designed as a browser-based utility.

Selected files are processed by the browser for the supported operations rather than being uploaded to a project-specific backend server.

```text
Your Computer
     │
     ▼
┌───────────────────┐
│   Chrome Browser  │
│                   │
│  Select PDF       │
│       ↓           │
│  Process locally  │
│       ↓           │
│  Download result  │
└───────────────────┘
```

> **Important:** The application loads its PDF processing libraries from external CDN URLs when the page loads. Internet access may therefore be required for the first load or whenever those libraries are not cached.

---

# 🌐 External Libraries

The current web application uses browser-loaded libraries including:

```text
PDF-LIB
PDF.js
JSZip
```

These libraries provide the core PDF manipulation, rendering, and ZIP functionality.

---

# 💻 Requirements

### Windows

- Windows 10 / 11
- Google Chrome, Microsoft Edge, or another modern browser

### Other Platforms

The HTML application can also be opened on other desktop operating systems with a modern browser.

No Python installation is required for the browser application.

---

# 🧪 Example Workflow

Suppose you have:

```text
assignment-part-1.pdf
assignment-part-2.pdf
assignment-part-3.pdf
```

Choose:

```text
📑 Merge PDFs
```

Then:

```text
Select Files
      ↓
assignment-part-1.pdf
assignment-part-2.pdf
assignment-part-3.pdf
      ↓
Merge & Download
      ↓
merged.pdf
```

---

# 🎨 Design

PDF Toolbox uses a modern dark interface with a purple glass-style visual theme.

Design goals:

- Clean
- Simple
- Modern
- Easy file selection
- Minimal controls
- Responsive layout
- Beginner-friendly workflow

---

# 🔮 Future Improvements

Possible future features:

- [ ] True PDF password encryption
- [ ] Better PDF compression
- [ ] PDF page reordering
- [ ] Rotate pages
- [ ] Delete pages
- [ ] Duplicate pages
- [ ] PDF metadata editor
- [ ] Page numbering
- [ ] Header / footer
- [ ] Image quality controls
- [ ] Custom PDF page sizes
- [ ] Batch processing
- [ ] PDF preview thumbnails
- [ ] Dark / light themes
- [ ] Offline bundled libraries
- [ ] Desktop `.exe` version
- [ ] Mobile-optimized version

---

# 🚀 Roadmap

### Version 1.0

```text
✓ Modern PDF Toolbox UI
✓ Merge PDFs
✓ Split PDFs
✓ Extract pages
✓ PDF optimization
✓ Images → PDF
✓ PDF → Images
✓ Text watermark
✓ Drag-and-drop upload
✓ Browser-based downloads
```

### Version 2.0

```text
□ Password encryption
□ Page management
□ PDF preview
□ Page reordering
□ Rotate / delete pages
□ Better compression
□ Metadata tools
```

### Version 3.0

```text
□ Offline bundled libraries
□ Standalone Windows EXE
□ Advanced PDF editor
□ Batch processing
□ Cross-platform desktop application
```

---

# 👨‍💻 Author

## Sam Wilson

**B.E. CSE — Artificial Intelligence & Machine Learning**

GitHub:

https://github.com/rsamwilson2323-cloud

---

# ⭐ Repository

**PDF_TOOLBOX**

https://github.com/rsamwilson2323-cloud/PDF_TOOLBOX

If you find the project useful, consider giving the repository a ⭐.

---

# 📜 License

This project is released under the **MIT License**.

See [`LICENSE`](LICENSE) for details.

---

# ⚡ Quick Start

```bash
git clone https://github.com/rsamwilson2323-cloud/PDF_TOOLBOX.git

cd PDF_TOOLBOX
```

Then open:

```text
PDF_TOOLBOX.html
```

or run:

```text
OPEN_PDF_TOOLBOX.bat
```

Choose a PDF task, select your files, and download the result.

---

### 📄 PDF → ⚡ Process → 💾 Download

**Simple. Fast. Browser-based.**
