# GPSC Final Boss: Personal Prep Tracker (Class 1/2)

A single-file, zero-dependency, private web application designed for candidates (especially those transitioning from engineering) preparing for the Gujarat Public Service Commission (GPSC) Class 1/2 examinations (targeting Deputy Collector / Gujarat Administrative Service).

---

## Features
- **Syllabus Tree:** Granular breakdown across Prelims and Mains subjects. Color-coded by mastery ($M < 0.4$ Red, $0.4 \le M \le 0.7$ Yellow, $M > 0.7$ Green, Grey for locked prerequisites).
- **"Study Now" Priority Engine:** Ranks topics in real-time using $P = W \times (1 - M) \times R \times D$, where $D = 1 + \text{days}/14$ (capped at 3.0), highlighting the top 5 focus areas with explicit rationale.
- **Mastery Scoring & Anti-Inflation:** Weights diagnostic quiz results at 70% and self-assessment at 30%.
- **Spaced-Repetition Revision Tracker:** Dynamic revision checkpoints at 1, 3, 7, 14, and 30 days.
- **Four-Phase Roadmap:** Foundation (Weeks 1–6), Core Mastery (Weeks 7–16), Mains Transition (Weeks 17–24), and Simulation (Weeks 25+).
- **PYQ Intelligence Engine:** Tag past exam questions by year, paper, and topic. Automatically recomputes topic weightages ($W$) from question counts.
- **Resource Vault (SSOT):** Strictly one editable "Single Source of Truth" resource per topic to eliminate material hoarding.
- **Readiness Matrix:** Visual subject mastery bars.
- **Zero-Backend & 100% Private:** State resides safely in browser `localStorage`. Includes Export JSON and Import JSON backup features.

---

## How to Run & Host
1. **Local Usage:** Simply double-click `index.html` or serve via any static HTTP server:
   ```bash
   python3 -m http.server 8000
   ```
   Open `http://localhost:8000`.
2. **Hosting:** Deploy `index.html` directly to **GitHub Pages**, **Cloudflare Pages**, or **Vercel** with zero build configuration needed.

---

> **⚠️ Disclaimer:** All marks, paper structures, book recommendations, and topic weightages in default data are unverified placeholders. Always verify against the latest official GPSC notification.
