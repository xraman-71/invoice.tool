<div align="center">

<img src="https://via.placeholder.com/80x80/0a0a0b/ffffff?text=IF" alt="Invoice.Tool Logo" width="80" height="80" style="border-radius:16px"/>

# InvoiceFlow

### Free Professional Invoice Generator — No Sign-Up. No Server. No Limits.

[![Version](https://img.shields.io/badge/version-1.0.0-0a0a0b?style=flat-square)](https://xraman-71.github.io/invoice.tool/))
[![License](https://img.shields.io/badge/license-MIT-0a0a0b?style=flat-square)](LICENSE)
[![Frontend Only](https://img.shields.io/badge/stack-100%25%20Frontend-0a0a0b?style=flat-square)](#)
[![Zero Data](https://img.shields.io/badge/data%20stored-0%20bytes-0a0a0b?style=flat-square)](#)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen?style=flat-square)](CONTRIBUTING.md)

[**🚀 Live Demo**](https://xraman-71.github.io/invoice.tool/) · [**📄 Create Invoice**](https://xraman-71.github.io/invoice.tool/) · [**🐛 Report Bug**](https://github.com/xraman-71/)

---

</div>

---

## 📌 Table of Contents

- [About](#-about)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Getting Started](#-getting-started)
- [File Structure](#-file-structure)
- [How It Works](#-how-it-works)
- [SEO & Performance](#-seo--performance)
- [Contributing](#-contributing)
- [Roadmap](#-roadmap)
- [License](#-license)

---

## 🧾 About

**InvoiceFlow** is a fully client-side invoice generator that lets freelancers, small businesses, and professionals create beautiful, professional PDF and Excel invoices — with zero friction.

> No account. No subscription. No data sent to any server. Ever.

Built with vanilla HTML, CSS, and JavaScript, InvoiceFlow is intentionally simple: open it in a browser, fill in your details, and download a polished invoice in under a minute.

---

## ✨ Features

| Feature | Description |
|---|---|
| 📋 **Smart Line Items** | Add unlimited products/services; Qty × Price calculates automatically |
| 💰 **Tax Configuration** | GST, VAT, or any custom % — computed and displayed separately |
| 📄 **PDF Export** | Download a print-ready, professional PDF invoice |
| 📊 **Excel / CSV Export** | Export to `.xlsx` or `.csv` for accounting software |
| 🔍 **Live Preview** | Real-time invoice preview as you type |
| 🛡️ **Field Validation** | Prevents export if required fields are missing |
| 📱 **Mobile Responsive** | Works on any device — phone, tablet, desktop |
| 🔢 **Auto Invoice Numbers** | Auto-generated, fully editable invoice ID sequence |
| 🌍 **Global Currency** | Supports USD, EUR, GBP, INR, and any currency symbol |
| ❤️ **100% Free Forever** | No paywalls, no watermarks, no ads |

---

## 🛠 Tech Stack

InvoiceFlow uses zero external frameworks or build tools. Everything runs in the browser.

```
HTML5          — Semantic, accessible markup
CSS3           — Custom properties, Grid, Flexbox, animations
Vanilla JS     — No frameworks, no dependencies
Canvas API     — Aurora background animation
IntersectionObserver API — Scroll-triggered reveal animations
```

**Fonts (via Google Fonts):**
- `Syne` — Display headings
- `Instrument Sans` — Body text
- `JetBrains Mono` — Monospaced labels and numbers

---
---

## 📁 File Structure

```
invoiceflow/
├── index.html          # Landing page (marketing site)
├── invoice-app.html    # Invoice creator application
├── favicon-32x32.png   # Favicon (replace with your own)
├── favicon-16x16.png
├── apple-touch-icon.png
├── og-image.png        # Open Graph social share image (1200×630)
├── site.webmanifest    # PWA manifest
└── README.md
```

> **Note:** All logic is self-contained within each HTML file. There are no external JS/CSS files, no node_modules, and no build pipeline.

---

## 🔄 How It Works

```
User opens invoice-app.html
        │
        ▼
Fills in: Business Info → Client Info → Line Items → Tax Rate
        │
        ▼
JS calculates: subtotal, tax amount, total due (live)
        │
        ▼
User clicks "Preview" → sees rendered invoice in-browser
        │
        ├──► "Download PDF"   → jsPDF renders and triggers download
        └──► "Export Excel"   → SheetJS builds .xlsx and triggers download
```

No data is ever transmitted. All processing happens locally in the browser session.

---

## 🔎 SEO & Performance

The SEO-optimized landing page (`index.html`) includes:

- **Semantic HTML5** — `<main>`, `<section>`, `<article>`, `<nav>`, `<footer>` with `aria-label` attributes
- **Structured Data (JSON-LD):**
  - `WebApplication` schema with full feature list and pricing
  - `FAQPage` schema for Google rich results
  - `BreadcrumbList` for site navigation
- **Open Graph tags** — optimized for Facebook, LinkedIn, WhatsApp previews
- **Twitter Card** — `summary_large_image` format
- **Canonical URL** — prevents duplicate content issues
- **Meta description** — keyword-rich, under 160 characters
- **`robots` meta** — `index, follow` with max-snippet and image preview hints
- **Accessible markup** — ARIA roles and labels throughout
- **FAQ accordion** — inline `itemscope`/`itemprop` microdata for Google rich snippets

### Lighthouse Targets

| Metric | Target |
|---|---|
| Performance | 95+ |
| Accessibility | 95+ |
| Best Practices | 100 |
| SEO | 100 |

---

## 🤝 Contributing

Contributions are welcome! Here's how to get started:

1. **Fork** the repository
2. **Create** a feature branch: `git checkout -b feature/your-feature-name`
3. **Commit** your changes: `git commit -m "feat: add your feature"`
4. **Push** to the branch: `git push origin feature/your-feature-name`
5. **Open** a Pull Request

### Guidelines

- Keep the zero-dependency philosophy — no npm packages, no bundlers
- Ensure all new UI is responsive (mobile-first)
- Test in Chrome, Firefox, Brave, and Edge before submitting
- Follow the existing code style (CSS custom properties, BEM-like naming)

---

## 🗺 Roadmap

- [ ] **Multi-language support** — invoice templates in Spanish, French, Hindi, Arabic
- [ ] **Logo upload** — add your company logo to the invoice header
- [ ] **Color themes** — choose invoice accent color / template style
- [ ] **Payment terms presets** — "Net 15", "Net 30", "Due on Receipt" quick-fill
- [ ] **Dark mode** — system-preference aware dark theme
- [ ] **Print-optimized CSS** — direct `window.print()` as alternative to PDF export
- [ ] **QR code for payment links** — embed UPI / PayPal link as QR
- [ ] **Offline PWA** — full service worker for offline-first use
- [ ] **Invoice history** — localStorage-based draft saving

---

## 📄 License

```
MIT License

Copyright (c) 2026 AMANXR-71

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND.
```

---

<div align="center">

Made with ♥ by **AMANXR**

[⭐ Star this repo](https://github.com/AMANXR/invoiceflow) if InvoiceFlow saved you time!

</div>
