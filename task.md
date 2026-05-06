# GitHub Copilot Prompt — Elite Cybersecurity Student Portfolio
# Vite + React + Plain CSS | Dark Hacker Aesthetic | Parallax & Scroll FX

> **Paste everything inside the triple-backtick block into GitHub Copilot Chat.**
> After generation, edit ONE file only — `src/data/portfolio.json` — to make it yours.

---

```
You are a senior frontend engineer and award-winning UI/UX designer.
Build me a WORLD-CLASS, jaw-dropping student portfolio website.

This is not a basic portfolio. This must look and feel like a premium
cybersecurity agency site — dark, atmospheric, cinematic, technically
impressive. Think: Awwwards-worthy. Every scroll should feel intentional.
Every hover should feel alive. Every section should make someone stop and say "wow."

The design language is: DARK TERMINAL × EDITORIAL LUXURY.
Inspired by the second reference image — near-black backgrounds, high-contrast
orange/red accent cuts, geometric grid overlays, brutalist typography, and
animated wireframe sphere/globe visuals built in pure CSS/SVG.

════════════════════════════════════════════════════════════
TECH STACK (strict — do not deviate)
════════════════════════════════════════════════════════════

- Vite + React (JSX)
- Plain CSS only — NO Tailwind, NO styled-components, NO UI libraries
- NO react-router-dom — single page, section-based scroll navigation
- Smooth scroll between anchor sections (CSS scroll-behavior: smooth)
- Google Fonts loaded in index.html
- Intersection Observer API for scroll-triggered animations (vanilla JS in useEffect)
- Parallax via CSS transform + JS scroll listener (requestAnimationFrame, passive)
- Custom animated cursor (CSS + JS)
- All personal data lives in ONE file: src/data/portfolio.json

════════════════════════════════════════════════════════════
COMPLETE FILE STRUCTURE
════════════════════════════════════════════════════════════

portfolio/
├── index.html                      ← Google Fonts, meta tags, favicon emoji 🛡️
├── vite.config.js
├── package.json
├── README.md                       ← full setup + customisation guide
└── src/
    ├── main.jsx
    ├── App.jsx                     ← assembles all sections, custom cursor
    ├── index.css                   ← CSS variables, reset, global styles, cursor
    ├── data/
    │   └── portfolio.json          ← ALL personal content lives here
    ├── components/
    │   ├── Navbar/
    │   │   ├── Navbar.jsx          ← sticky top nav, logo, nav links, CTA
    │   │   └── Navbar.css
    │   ├── CustomCursor/
    │   │   ├── CustomCursor.jsx    ← animated dot + ring cursor
    │   │   └── CustomCursor.css
    │   ├── GlobeCanvas/
    │   │   ├── GlobeCanvas.jsx     ← animated wireframe sphere in pure SVG/CSS
    │   │   └── GlobeCanvas.css
    │   └── ScrollReveal/
    │       └── useScrollReveal.js  ← custom hook: IntersectionObserver reveal
    └── sections/
        ├── Hero/
        │   ├── Hero.jsx            ← fullscreen, parallax, animated tagline
        │   └── Hero.css
        ├── Marquee/
        │   ├── Marquee.jsx         ← scrolling ticker: tools & tech logos as text
        │   └── Marquee.css
        ├── About/
        │   ├── About.jsx
        │   └── About.css
        ├── Skills/
        │   ├── Skills.jsx
        │   └── Skills.css
        ├── Projects/
        │   ├── Projects.jsx
        │   └── Projects.css
        ├── Timeline/
        │   ├── Timeline.jsx        ← education & certifications
        │   └── Timeline.css
        ├── Contact/
        │   ├── Contact.jsx
        │   └── Contact.css
        └── Footer/
            ├── Footer.jsx
            └── Footer.css

════════════════════════════════════════════════════════════
src/data/portfolio.json  — THE ONLY FILE A STUDENT EDITS
════════════════════════════════════════════════════════════

Create this exact JSON structure. Comments explain each field:

{
  "identity": {
    "name": "Alex Carter",
    "initials": "AC",
    "tagline": "Cybersecurity Student & Ethical Hacker",
    "degree": "BSc Cybersecurity",
    "level": "Level 5 — Year 2",
    "university": "University of Greenwich",
    "location": "London, UK",
    "status": "Open for Internships",
    "statusActive": true,
    "bio": [
      "I'm a second-year Cybersecurity student obsessed with breaking things ethically — then building them stronger. My playground is the intersection of network defence, exploit development, and CTF competition.",
      "When I'm not studying packets or reverse-engineering binaries, I'm contributing to open-source security tools and documenting my CTF write-ups for the community."
    ],
    "heroHeadline": "Threats require advanced solutions.",
    "heroSub": "BSc Cybersecurity · Ethical Hacking · Network Defence"
  },
  "contact": {
    "email": "alex@example.com",
    "github": "github.com/alexcarter",
    "linkedin": "linkedin.com/in/alexcarter",
    "twitter": "@alexcarter_sec"
  },
  "skills": [
    {
      "category": "Offensive Security",
      "items": [
        { "name": "Metasploit", "level": 80 },
        { "name": "Burp Suite", "level": 85 },
        { "name": "Nmap / Masscan", "level": 90 },
        { "name": "SQLMap", "level": 75 }
      ]
    },
    {
      "category": "Programming",
      "items": [
        { "name": "Python", "level": 85 },
        { "name": "Bash / Shell", "level": 80 },
        { "name": "C / C++", "level": 60 },
        { "name": "JavaScript", "level": 65 }
      ]
    },
    {
      "category": "Concepts & Tools",
      "items": [
        { "name": "Network Protocols", "level": 88 },
        { "name": "Cryptography", "level": 72 },
        { "name": "OSINT", "level": 82 },
        { "name": "Wireshark", "level": 90 }
      ]
    }
  ],
  "projects": [
    {
      "id": 1,
      "title": "Network Packet Analyser",
      "description": "A real-time Python tool for deep packet inspection and traffic visualisation on local networks. Exports to PCAP and generates summary threat reports.",
      "tags": ["Python", "Scapy", "Wireshark", "SQLite"],
      "github": "#",
      "live": "#",
      "featured": true
    },
    {
      "id": 2,
      "title": "CTF Write-up Archive",
      "description": "Documented solutions and methodology breakdowns for 25+ CTF competitions across HackTheBox, TryHackMe, and PicoCTF. Organised by category and difficulty.",
      "tags": ["Linux", "OSINT", "Reverse Engineering", "Web Exploitation"],
      "github": "#",
      "live": "#",
      "featured": true
    },
    {
      "id": 3,
      "title": "Auto Vulnerability Scanner",
      "description": "Automated multi-threaded scanner that runs Nmap, checks CVE databases, and generates PDF vulnerability reports for small business network audits.",
      "tags": ["Python", "Nmap", "REST API", "ReportLab"],
      "github": "#",
      "live": null,
      "featured": false
    },
    {
      "id": 4,
      "title": "E2E Encrypted Chat",
      "description": "Peer-to-peer encrypted messaging application using RSA for key exchange and AES-256-GCM for message encryption. No server stores message content.",
      "tags": ["Python", "Cryptography", "Sockets", "Tkinter"],
      "github": "#",
      "live": null,
      "featured": false
    }
  ],
  "timeline": [
    {
      "year": "2024 – Present",
      "title": "BSc Cybersecurity — Level 5",
      "org": "University of Greenwich",
      "type": "education"
    },
    {
      "year": "2024",
      "title": "CompTIA Security+ (in progress)",
      "org": "CompTIA",
      "type": "cert"
    },
    {
      "year": "2023",
      "title": "BSc Cybersecurity — Level 4",
      "org": "University of Greenwich",
      "type": "education"
    },
    {
      "year": "2023",
      "title": "Google Cybersecurity Certificate",
      "org": "Google / Coursera",
      "type": "cert"
    }
  ],
  "marquee": [
    "Wireshark", "Metasploit", "Kali Linux", "Burp Suite",
    "Python", "Nmap", "CTF", "OSINT", "Cryptography",
    "Network Security", "Ethical Hacking", "TryHackMe", "HackTheBox"
  ]
}

════════════════════════════════════════════════════════════
DESIGN SYSTEM — index.css
════════════════════════════════════════════════════════════

:root {
  /* Palette */
  --bg:           #0a0a0a;      /* near-black background */
  --bg-2:         #111111;      /* slightly lifted surface */
  --bg-3:         #1a1a1a;      /* card surfaces */
  --accent:       #ff4500;      /* electric orange-red (cyber threat colour) */
  --accent-dim:   rgba(255,69,0,0.12);
  --accent-glow:  rgba(255,69,0,0.35);
  --text:         #f0ede8;      /* warm off-white — not pure white */
  --text-muted:   #6b6b6b;
  --border:       rgba(255,255,255,0.07);
  --border-hot:   rgba(255,69,0,0.4);

  /* Typography */
  --font-display: 'Bebas Neue', 'Impact', sans-serif;   /* headlines */
  --font-body:    'Sora', system-ui, sans-serif;         /* body copy */
  --font-mono:    'JetBrains Mono', 'Courier New', monospace; /* code/labels */

  /* Motion */
  --ease-out-expo: cubic-bezier(0.16, 1, 0.3, 1);
  --ease-in-out:   cubic-bezier(0.87, 0, 0.13, 1);
  --dur-fast:      0.2s;
  --dur-med:       0.5s;
  --dur-slow:      0.9s;

  /* Geometry */
  --max-w:   1280px;
  --section-pad: 140px 0;
}

Load in index.html <head>:
  <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Sora:wght@300;400;600&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet">

Global rules:
- html { scroll-behavior: smooth; }
- body { background: var(--bg); color: var(--text); overflow-x: hidden; cursor: none; }
- ::selection { background: var(--accent); color: #000; }
- Thin 1px horizontal grid lines as repeating background on body (subtle, 10% opacity):
  background-image: repeating-linear-gradient(0deg, transparent, transparent 79px, rgba(255,255,255,0.03) 80px);
- Scrollbar: thin, accent-coloured:
  ::-webkit-scrollbar { width: 3px; }
  ::-webkit-scrollbar-thumb { background: var(--accent); }

════════════════════════════════════════════════════════════
COMPONENT — CustomCursor
════════════════════════════════════════════════════════════

Two DOM elements: .cursor-dot (6px filled circle) + .cursor-ring (32px hollow ring).
- Both positioned fixed, pointer-events: none, z-index: 9999
- dot follows mouse instantly via JS (mousemove → transform: translate)
- ring follows with 80ms lerp delay (requestAnimationFrame interpolation)
- On hover over any <a>, <button>: ring scales to 2× and turns --accent colour
- On mousedown: dot scales to 0.5×
- Implement lerp: next = curr + (target - curr) * 0.12 per frame

════════════════════════════════════════════════════════════
COMPONENT — GlobeCanvas
════════════════════════════════════════════════════════════

Animated wireframe globe built in pure SVG + CSS — NO canvas, NO Three.js, NO libraries.

Technique:
- A set of 8 ellipses rotated at different angles (longitude lines) to form a sphere
- 4 horizontal ellipses (latitude rings) scaled by sin() to give sphere shape
- All strokes: var(--accent) at 0.3–0.6 opacity
- CSS animation rotates the whole group slowly (60s linear infinite)
- A second counter-rotation on inner rings creates depth illusion
- Optional: CSS @keyframes pulsing glow on the globe (filter: drop-shadow)
- Globe is 400×400px SVG viewBox, scales with container

Use the globe in the Hero section (right column) and in project card backgrounds (smaller, 15% opacity).

════════════════════════════════════════════════════════════
SECTION — Navbar
════════════════════════════════════════════════════════════

- Fixed top, full width, z-index 100
- Background: rgba(10,10,10,0.85) + backdrop-filter: blur(20px) saturate(180%)
- Bottom border: 1px solid var(--border)
- Left: initials badge — square 36px, accent background, mono font: "AC"
- Right: nav links — Home | About | Skills | Projects | Timeline | Contact
  Links are uppercase, mono font, 0.8rem, letter-spacing: 0.15em
  Active link: accent colour + underline that slides in from left (CSS ::after pseudo)
- Far right: pill badge "[STATUS]" — amber if statusActive, grey if false
- On scroll > 50px: navbar shrinks slightly (padding reduces, CSS transition)
- Nav links are <a href="#sectionId"> for smooth scroll to anchor sections

════════════════════════════════════════════════════════════
SECTION — Hero (fullscreen, parallax)
════════════════════════════════════════════════════════════

Layout: two-column (60/40 split) — text left, globe right.
Height: 100vh minimum.
Background: var(--bg) with a diagonal orange slash overlay (CSS clip-path polygon,
  5% opacity — a subtle nod to the reference design).

Left column content:
  - Small mono label (blinking cursor animation): "> CYBERSECURITY STUDENT_"
  - Giant headline from data.heroHeadline rendered in --font-display,
    font-size clamp(56px, 8vw, 130px), line-height 0.9, uppercase
    First half: var(--text), key word (e.g. "threats"): var(--accent)
  - Subtitle: data.heroSub — mono font, muted colour, letter-spacing wide
  - Two CTA buttons:
      [VIEW MY WORK ↓]  — filled accent background, black text
      [DOWNLOAD CV]     — outlined, accent border, accent text
  - Small stat row: "25+ CTFs | 4 Projects | BSc Cyber"
    mono font, separated by thin vertical lines

Right column:
  - GlobeCanvas component, size 460px
  - Subtle radial glow behind globe: var(--accent-glow) blurred 120px

Parallax: On scroll, left column moves at 0.3× scroll speed (translateY),
  globe moves at -0.15× (opposite direction). Use requestAnimationFrame.

Page-load animation sequence (stagger with CSS animation-delay):
  1. Navbar slides down from -60px → 0 (0.4s)
  2. Label fades in (0.6s delay)
  3. Headline animates letter by letter: each word slides up from translateY(100%) (0.8s delay, stagger 0.1s per word using JS split + inline style)
  4. Subtitle + buttons fade in (1.2s delay)
  5. Globe fades in + scales from 0.8 → 1 (1.0s delay)

════════════════════════════════════════════════════════════
SECTION — Marquee (ticker tape)
════════════════════════════════════════════════════════════

Full-width horizontal scrolling ticker between Hero and About.
Background: var(--accent), height: 48px.
Content: portfolio.json marquee array, repeated 3× for seamless loop.
CSS animation: translateX(-33.33%) in 25s linear infinite.
Text: uppercase, --font-mono, black (#000), font-size 0.85rem, letter-spacing 0.2em.
Each item separated by " · " in accent colour (but inverted since bg is accent: use black dot).
On hover: animation-play-state: paused.

════════════════════════════════════════════════════════════
SECTION — About (id="about")
════════════════════════════════════════════════════════════

Two-column layout. Padding: var(--section-pad).
Left (45%): large text "ABOUT ME" in display font, stacked vertically with huge
  font-size (clamp 80px–160px) rotated 90deg, used as decorative label (opacity 0.04).
  Then actual heading: "Who Am I?"
  Bio paragraphs from data.identity.bio, body font, line-height 1.8.
  Below bio: row of interest tags (pill chips, var(--accent) border, transparent bg).

Right (55%): Info card grid (2×2):
  ┌─────────────────┬─────────────────┐
  │  DEGREE         │  LEVEL          │
  │  BSc Cybersec   │  Level 5 · Yr2  │
  ├─────────────────┼─────────────────┤
  │  UNIVERSITY     │  LOCATION       │
  │  [value]        │  [value]        │
  └─────────────────┴─────────────────┘
  Cards: bg var(--bg-3), border var(--border), subtle top accent line (3px var(--accent))
  Label: --font-mono, muted, uppercase, 0.7rem
  Value: --font-display, large, var(--text)

Scroll reveal: left column slides in from left (-60px → 0), right column from right.

════════════════════════════════════════════════════════════
SECTION — Skills (id="skills")
════════════════════════════════════════════════════════════

Full-width dark section (bg: var(--bg-2)).
Header: "TECHNICAL ARSENAL" in display font, centred, massive (clamp 60px, 10vw, 120px),
  text barely visible at opacity 0.06 behind the actual content (layered headings technique).
  Real heading: "Skills" smaller, accent coloured.

Three columns, each rendered from data.skills array.
Category title: --font-mono, uppercase, accent colour, small.
Each skill item:
  - Name: body font, left
  - Percentage number: mono font, accent colour, right
  - Progress bar: full width, height 2px, bg rgba(255,255,255,0.08)
    Filled portion: var(--accent) gradient, width animates from 0 → level% when
    section enters viewport (IntersectionObserver triggers CSS custom property update).
  - Hover: bar glows with var(--accent-glow) drop shadow.

════════════════════════════════════════════════════════════
SECTION — Projects (id="projects")
════════════════════════════════════════════════════════════

Header same layered technique as Skills: "PROJECTS" ghost text + real heading.

Featured projects (featured: true): full-width bento cards stacked.
  Each card: horizontal layout — text left 55%, visual right 45%.
  Visual: large project number ("01", "02") in display font at 30% opacity
    + small GlobeCanvas (160px, 10% opacity) overlaid.
  Card bg: var(--bg-3). Left 4px border: var(--accent) on hover (CSS transition).
  Content: title (display font, large), description, tech tag chips, buttons.
  Button styles: outlined ghost button + filled accent button.
  Hover on card: subtle translateY(-4px), border colour animates to accent.

Regular projects (featured: false): 2-column grid of smaller cards.
  Same style but compact, text-only (no globe visual).

Scroll reveal: cards alternate — odd slides from left, even from right.

════════════════════════════════════════════════════════════
SECTION — Timeline (id="timeline")
════════════════════════════════════════════════════════════

Vertical timeline centred on page.
Centre spine: 2px line, var(--accent) colour, grows from top (CSS scaleY animation
  triggered by IntersectionObserver — height animates 0 → 100%).

Each timeline item alternates left / right of the centre line.
Item dot: 12px circle, accent filled, on the centre line.
Item card: bg var(--bg-3), border var(--border), slight border-radius.
  Year: --font-mono, accent, bold.
  Title: body font, white, 1.1rem.
  Org: muted, mono, small.
  Type badge: "EDUCATION" or "CERT" — pill, different colours (accent vs green #22c55e).

Items animate in as the line grows.

════════════════════════════════════════════════════════════
SECTION — Contact (id="contact")
════════════════════════════════════════════════════════════

Two-column layout.
Left (45%):
  Giant display text "LET'S WORK" on one line, "TOGETHER." on the next.
  font-size: clamp(40px, 6vw, 90px).
  Below: short paragraph: "I'm open to internships, freelance security consulting,
  and collaborative CTF teams."
  Social links: GitHub | LinkedIn | Twitter — each with → arrow icon (unicode →),
  mono font, accent colour on hover, slide-right animation.

Right (55%): contact form.
  Fields: Name, Email, Message (textarea).
  All fields: borderless, only a bottom border (2px var(--border)).
  On focus: bottom border animates to var(--accent), label floats above (CSS :focus-within).
  Submit button: full-width, accent background, "SEND MESSAGE →" in bold mono.
  Button hover: background darkens, slight translateY(-2px).
  Success state: form replaced with large checkmark animation + "Message sent. I'll be in touch."

════════════════════════════════════════════════════════════
COMPONENT — Footer
════════════════════════════════════════════════════════════

Full-width, very thin strip. bg: var(--bg-2). Border-top: 1px var(--border).
Padding: 24px 0.
Three columns:
  Left: initials badge + name + degree (small mono text)
  Centre: "BUILT WITH REACT + VITE" mono text, very muted
  Right: "© 2025 Alex Carter" + nav links (small, no decoration)

════════════════════════════════════════════════════════════
SCROLL REVEAL SYSTEM — useScrollReveal.js
════════════════════════════════════════════════════════════

Custom hook using IntersectionObserver:

export function useScrollReveal(options = {}) {
  const ref = useRef(null);
  useEffect(() => {
    const el = ref.current;
    if (!el) return;
    const obs = new IntersectionObserver(([entry]) => {
      if (entry.isIntersecting) {
        el.classList.add('revealed');
        obs.unobserve(el);
      }
    }, { threshold: 0.15, ...options });
    obs.observe(el);
    return () => obs.disconnect();
  }, []);
  return ref;
}

In index.css define:
.reveal { opacity: 0; transform: translateY(40px); transition: opacity 0.8s var(--ease-out-expo), transform 0.8s var(--ease-out-expo); }
.reveal.revealed { opacity: 1; transform: translateY(0); }
.reveal-left { opacity: 0; transform: translateX(-60px); transition: ... }
.reveal-left.revealed { opacity: 1; transform: translateX(0); }
.reveal-right { opacity: 0; transform: translateX(60px); transition: ... }
.reveal-right.revealed { opacity: 1; transform: translateX(0); }

Wrap every major section element in a <div className="reveal"> and attach the ref.

════════════════════════════════════════════════════════════
PARALLAX IMPLEMENTATION
════════════════════════════════════════════════════════════

In App.jsx, single scroll listener using requestAnimationFrame:

useEffect(() => {
  let ticking = false;
  const onScroll = () => {
    if (!ticking) {
      requestAnimationFrame(() => {
        const y = window.scrollY;
        const heroText = document.querySelector('.hero-text');
        const heroGlobe = document.querySelector('.hero-globe');
        if (heroText) heroText.style.transform = `translateY(${y * 0.3}px)`;
        if (heroGlobe) heroGlobe.style.transform = `translateY(${y * -0.15}px)`;
        ticking = false;
      });
      ticking = true;
    }
  };
  window.addEventListener('scroll', onScroll, { passive: true });
  return () => window.removeEventListener('scroll', onScroll);
}, []);

════════════════════════════════════════════════════════════
MOBILE RESPONSIVENESS
════════════════════════════════════════════════════════════

Single breakpoint at 768px. On mobile:
- Hero: single column, globe hidden (display: none), headline font-size 13vw
- Navbar: logo left, hamburger icon right (☰ / ✕ toggle — pure CSS checkbox hack or useState)
  Mobile nav: full-screen overlay, links centred, large, staggered fade-in
- About, Projects: single column
- Skills: single column
- Timeline: left-aligned only (no alternating)
- Contact: single column
- Custom cursor: disabled on touch devices (CSS @media (pointer: coarse))

════════════════════════════════════════════════════════════
README.md — write this full content
════════════════════════════════════════════════════════════

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

**Edit ONE file only:**

```
src/data/portfolio.json
```

Change every value in that file — your name, degree, skills, projects, links.
The entire website updates automatically.

**JSON sections explained:**
| Key | What to change |
|-----|---------------|
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
| `src/data/portfolio.json` | **All your personal data — edit this only** |
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

════════════════════════════════════════════════════════════
FINAL QUALITY CHECKLIST — verify before finishing
════════════════════════════════════════════════════════════

[ ] All personal data sourced exclusively from portfolio.json — zero hardcoded strings
[ ] Custom cursor works and is disabled on mobile/touch
[ ] Parallax runs on requestAnimationFrame with passive scroll listener
[ ] All sections have scroll-reveal animations via IntersectionObserver
[ ] GlobeCanvas is pure SVG/CSS — no canvas, no Three.js
[ ] Marquee loops infinitely and pauses on hover
[ ] Progress bars animate from 0 on scroll entry
[ ] Timeline centre line grows as user scrolls into section
[ ] Contact form shows success state (no backend needed)
[ ] Mobile nav works at 375px viewport
[ ] Google Fonts (Bebas Neue, Sora, JetBrains Mono) loaded in index.html
[ ] CSS custom properties used consistently for all colours, durations, easings
[ ] README includes full install steps, JSON guide table, and deploy instructions
[ ] No Tailwind, no styled-components, no external CSS frameworks
[ ] No react-router-dom — sections connected by anchor IDs and smooth scroll
[ ] package.json has correct scripts: dev, build, preview

Generate all files completely, one at a time, with full working code.
Start with: portfolio.json → index.css → index.html → App.jsx → then each component.
```

---

## What this generates vs the old prompt

| Feature | Old prompt | This prompt |
|---|---|---|
| Theme | Light/white cards | Dark cinematic, orange-red cyber |
| Data management | Comments in JSX | Single `portfolio.json` |
| Cursor | Default browser | Custom animated dot + ring |
| Parallax | None | Hero text + globe counter-parallax |
| Globe | None | Animated wireframe SVG sphere |
| Scroll animations | None | IntersectionObserver on every section |
| Marquee | None | Infinite scrolling ticker tape |
| Timeline | None | Animated growing vertical timeline |
| Mobile nav | Pills wrap | Full-screen overlay menu |
| README | Basic | Full install + deploy + JSON guide |