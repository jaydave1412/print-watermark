# Print Branding Watermark Demo

This project demonstrates how to add a **branding watermark (logo)** to an HTML document that:

- Appears **on screen and in print**
- Repeats automatically on **every printed page**
- Works correctly for **multi-page documents**
- Includes a **Print button** that is visible on screen but hidden during printing

This approach is ideal for **invoices, reports, challans, and internal documents** where branding is required but strict security is not.

---

## ✨ Features

- Centered logo watermark using pure CSS
- Watermark visible on HTML view and printed pages
- Automatically repeats on every page in multi-page prints
- Print button hidden during print
- No JavaScript required for watermarking
- Works in Chrome, Edge, and Firefox

---

## 📂 Project Structure

    .
    ├── index.html        # Main demo file
    ├── small.png      # Branding logo used as watermark
    └── README.md

---

## 🚀 How It Works

- The watermark is implemented using `body::before`
- `position: fixed` ensures the watermark repeats on each printed page
- Opacity is kept low for a professional, non-intrusive look
- `@media print` hides UI elements like the print button

Key CSS concept:

    body::before {
      position: fixed;
    }

---

## 🖨️ Printing Instructions

1. Open `index.html` in a modern browser (Chrome or Edge recommended)
2. Click the **Print** button
3. In the print dialog:
   - Enable **Background graphics** (required for logo watermark)
4. Print or save as PDF

---

## 🎨 Customization

### Change watermark size

    width: 300px;
    height: 300px;

### Change watermark opacity

    opacity: 0.05;  /* lighter */
    opacity: 0.1;   /* darker */

### Move watermark to a corner

    top: auto;
    left: auto;
    bottom: 20mm;
    right: 20mm;
    transform: none;

---

## ⚠️ Limitations

- This is a branding-only watermark
- CSS-based watermarks can be removed by advanced users
- Not suitable for legal or tamper-proof documents

For non-removable watermarks, use server-side PDF generation.

---

## ✅ Recommended Use Cases

- Invoices
- Reports
- Internal documents
- Client previews
- Branded printouts from web software

---

## 🙏 Attribution

Logo PNGs used in this project are provided by  
Vecteezy — https://www.vecteezy.com/free-png/logo
