# 🛡️ Cybersecurity Portfolio Template

A dark, cinematic portfolio template for cybersecurity students.
Built with Vite + React + plain CSS. No UI frameworks. No bloat.

## 🚀 Setup (5 minutes)

### Prerequisites
- Node.js 18+ → https://nodejs.org
- Git → https://git-scm.com

### Installation

```bash
# 1. Clone or download this repository
git clone https://github.com/your-username/portfolio.git
cd portfolio

# 2. Install dependencies
npm install

# 3. Start dev server
npm run dev

# 4. Open in browser
# → http://localhost:5173
```

### Build for production
```bash
npm run build
npm run preview
```

## ✏️ How to Make It Yours (2 minutes)

Edit ONE file only:

```text
src/data/portfolio.json
```

Change every value in that file — your name, degree, skills, projects, links.
The entire website updates automatically.

JSON sections explained:

| Key | What to change |
|------|---------|
| `identity` | Your name, tagline, university, bio |
| `contact` | Your email, GitHub, LinkedIn |
| `skills` | Your skill categories and levels (0-100) |
| `projects` | Your project titles, descriptions, tags, links |
| `timeline` | Your education history and certifications |
| `marquee` | The scrolling ticker keywords |

## 🌐 Deploy Free in 3 Minutes

### Vercel (recommended)
1. Push to GitHub
2. Go to vercel.com → Import project → select your repo
3. Click Deploy. Done. You get a free .vercel.app URL.

### GitHub Pages
```bash
npm install -D gh-pages
# Add to package.json scripts:  "deploy": "gh-pages -d dist"
npm run build && npm run deploy
```

## 📂 File Structure

| File | Purpose |
|------|---------|
| `src/data/portfolio.json` | All your personal data — edit this only |
| `src/index.css` | Design tokens / CSS variables |
| `src/sections/` | Page sections (Hero, About, Skills…) |
| `src/components/` | Shared components (Navbar, Globe, Cursor) |

## 🎨 Changing Colors

In `src/index.css` find `:root` and edit:
- `--accent`: main colour (default: orange-red #ff4500)
- `--bg`: background colour (default: near-black #0a0a0a)
- `--text`: text colour (default: warm white #f0ede8)

---
Template created for cybersecurity students. Free to use and adapt.
