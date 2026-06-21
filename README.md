# 🎬 Vidzeee by Azeee

A browser-based video shorts creator — upload one long video, split it into clips, add styled captions, and export real `.mp4` files. No server needed.

---

## ✨ Features

- **Video upload** — MP4, MOV, WebM up to 2GB
- **3 split modes** — equal parts, by clip duration, or custom cut points
- **Caption editor** — per-clip text, font family, color, background, size, weight, position & style (shadow / outline / glow)
- **FFmpeg.wasm export** — real `.mp4` downloads with captions burned in, runs entirely in the browser
- **YouTube SRT Downloader** — paste a YouTube link to grab subtitle files
- **No backend, no login, no cost**

---

## 🚀 Deploy in 1 minute

### Option 1 — GitHub Pages (free, recommended)
1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Your site will be live at `https://yourusername.github.io/vidzeee`

### Option 2 — Netlify (free, instant)
1. Go to [netlify.com](https://netlify.com)
2. Drag and drop this entire folder onto the Netlify dashboard
3. Done — live URL in seconds

### Option 3 — Vercel (free)
1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` inside this folder
3. Follow the prompts

### Option 4 — Just open locally
Double-click `index.html` — works instantly in Chrome or Edge.

> **Note:** FFmpeg.wasm works best in **Chrome** or **Edge**. Firefox may have limited SharedArrayBuffer support.

---

## 📁 File Structure

```
vidzeee/
├── index.html      ← entire app (single file)
└── README.md       ← this file
```

---

## 🛠 Tech Stack

| Layer | Tech |
|---|---|
| UI | Vanilla HTML + CSS + JS |
| Video processing | FFmpeg.wasm 0.11.6 (via CDN) |
| Fonts | Google Fonts (Inter + Space Grotesk) |
| SRT download | downsub.com (external) |

---

## ⚠️ Browser Notes

- Chrome / Edge: full FFmpeg.wasm support ✅
- Firefox: may fall back to WebM export via MediaRecorder
- Safari: limited support, basic export only
- Mobile: not recommended for large files

---

Made with ❤️ by Azeee
