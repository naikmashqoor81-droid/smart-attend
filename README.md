# SmartAttend — AI-Powered Attendance System

> Hackathon project: "AI in Attendance" | Built with ai and dedication

![SmartAttend](https://img.shields.io/badge/AI-Claude%20Sonnet-4ade80?style=flat-square) ![Status](https://img.shields.io/badge/Status-Live-22d3ee?style=flat-square) ![License](https://img.shields.io/badge/License-MIT-f97316?style=flat-square)

## What It Does

SmartAttend is a single-file web app that lets teachers mark and track student attendance — with real AI features powered by Claude (Anthropic) that solve actual classroom problems:

| Feature | Description |
|---|---|
| **Mark Attendance** | Click P / A / L (Present / Absent / Late) per student per session |
| **Dashboard** | Live attendance rates, progress bars, at-risk flags |
| **AI: At-Risk Detector** | Claude analyzes all students, flags those below 75% with recommendations |
| **AI: Weekly Summary** | One-click professional summary paragraph for the teacher |
| **AI: Parent Notice** | Auto-drafts a polite parent notification for the lowest-attendance student |
| **AI: Excuse Validator** | Teacher submits a student excuse, Claude classifies it as Genuine / Suspicious / Needs Verification |

## Live Demo

Open `index.html` in any browser — no server, no install needed.

1. Get a free API key from [console.anthropic.com](https://console.anthropic.com)
2. Paste it in the top-right input
3. Click any AI button on the right panel

## Setup (30 seconds)

```bash
git clone https://github.com/YOUR_USERNAME/smartattend
cd smartattend
# Open index.html in your browser
```

No npm. No build step. No backend. Everything runs client-side.

## Tech Stack

- **Frontend**: Pure HTML + CSS + Vanilla JS (zero dependencies)
- **AI**: Anthropic Claude API (`claude-sonnet-4-20250514`)
- **Storage**: In-memory (easy to extend with localStorage or a backend)
- **Deploy**: GitHub Pages (one click)

## Deploy to GitHub Pages

1. Push this repo to GitHub
2. Go to Settings → Pages → Source: `main` branch → `/root`
3. Your app is live at `https://YOUR_USERNAME.github.io/smartattend`

## Project Structure

```
smartattend/
└── index.html    # Complete app — all HTML, CSS, JS in one file
└── README.md
```

## AI Prompts Used

The app makes 4 types of Claude API calls:

```js
// 1. At-Risk Detection
"Analyze attendance data, identify students below 75%, give recommendations"

// 2. Weekly Summary  
"Write a 3-4 sentence professional weekly attendance summary for a teacher"

// 3. Parent Notice
"Draft a polite parent notification letter for student with X% attendance"

// 4. Excuse Validation
"Classify this absence excuse as GENUINE / SUSPICIOUS / NEEDS-VERIFICATION"
```

## Screenshots

> Dashboard with live stats and progress bars  
> Mark Attendance with P/A/L cards  
> AI panel with real-time Claude responses

## Built For

**Hackathon Theme**: AI in Attendance  
**Developer**: Solo project  
**Time**: Built in ~3 hours

---

MIT License
