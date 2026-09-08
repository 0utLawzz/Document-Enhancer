# Document Enhancer (DocBright)

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-19-61DAFB?logo=react&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-646CFF?logo=vite&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/Hosted-GitHub%20Pages-222?logo=github)
![Status](https://img.shields.io/badge/Status-Active-success)

> Privacy-first browser document enhancer — improve scanned documents and photos entirely on-device. No uploads, no server, no cloud.

**Live demo:** [https://0utlawzz.github.io/Document-Enhanser/](https://0utlawzz.github.io/Document-Enhanser/)

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Project Structure](#project-structure)
- [Deployment](#deployment)
- [Suggested Improvements](#suggested-improvements)
- [License](#license)
- [Author](#author)

---

## Overview

Document Enhancer (branded **DocBright** in the web app) is a client-side tool for cleaning up scanned documents and photos. All processing happens in the browser; images never leave the device. It is intended as a lightweight CamScanner-style utility with batch support and ZIP export.

---

## Features

| Feature | Description |
|---------|-------------|
| Privacy-first | 100% local — no uploads, no server processing |
| Enhancement presets | Print Ready, B&W, Photo Recovery, and additional modes |
| Batch processing | Process multiple images in one session |
| ZIP export | Download the full set as a single archive |
| Modern UI | Dark neon styling with glass panels and micro-animations |
| Responsive | Works on desktop and mobile browsers |

---

## Tech Stack

| Layer | Technology |
|-------|------------|
| Frontend | React 19, TypeScript, Vite |
| UI | Tailwind CSS, Radix UI, Framer Motion, Lucide |
| Utilities | JSZip, Wouter, Zod, React Hook Form |
| Hosting | GitHub Pages (workflow present) |

---

## Installation

### Prerequisites

- Node.js 20+
- npm or pnpm (workspace-aware)

### Local development

```bash
git clone https://github.com/0utLawzz/Document-Enhanser.git
cd Document-Enhanser

# From the web app package
cd artifacts/docbright-web
npm install
npm run dev
```

Open the URL printed by Vite (typically `http://localhost:5173`).

### Production build

```bash
cd artifacts/docbright-web
npm run build
npm run typecheck
```

---

## Project Structure

```text
artifacts/
├── docbright-web/     # Main React + Vite application
│   ├── src/App.tsx    # Primary UI and enhancement flow
│   ├── src/components/
│   └── public/
└── api-server/        # Optional / scaffold API (not required for client-only mode)
.github/workflows/     # GitHub Pages deploy workflow
```

---

## Deployment

GitHub Pages is configured via `.github/workflows/deploy.yml`.  
Live URL: **https://0utlawzz.github.io/Document-Enhanser/**

---

## Suggested Improvements

| Priority | Item |
|----------|------|
| Medium | Correct repository name spelling (`Enhanser` → `Enhancer`) if desired |
| Medium | Expand unit tests around image-processing pipelines |
| Low | Add before/after comparison slider |
| Low | Optional OCR (client-side) for searchable PDFs |
| Info | Community files (LICENSE, CODE_OF_CONDUCT, CONTRIBUTING, issue templates) already present |

---

## License

MIT — see [LICENSE](LICENSE).

---

## Author

**Nadeem (OutLawZ)**  
Custom Automation Specialist  

- GitHub: [0utLawzz](https://github.com/0utLawzz)  
- Contact: net2outlawzz@gmail.com  

---

*Need custom document enhancement or image automation? Contact me.*
