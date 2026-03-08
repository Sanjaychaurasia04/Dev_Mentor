#  DevMentor — Learn to Code. For India.

<div align="center">

**An AI-powered coding education platform built for Indian developers — in their language, for their market.**

[![Made with React](https://img.shields.io/badge/Made%20with-React%2018-61dafb?style=flat-square&logo=react)](https://react.dev)
[![Powered by Groq](https://img.shields.io/badge/AI-Groq%20LLaMA%203.3-f97316?style=flat-square)](https://groq.com)
[![AWS Bedrock](https://img.shields.io/badge/AWS-Bedrock-232f3e?style=flat-square&logo=amazon-aws)](https://aws.amazon.com/bedrock/)
[![Single File](https://img.shields.io/badge/Deploy-Single%20HTML%20File-14b8a6?style=flat-square)]()
[![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)]()

###  [Live Demo → dev-mentor-s3.s3.eu-north-1.amazonaws.com/index.html](https://dev-mentor-s3.s3.eu-north-1.amazonaws.com/index.html)

<br />

> Built for the **AI for Bharat Hackathon** · Powered by **Claude + AWS Bedrock**  
> *भारत के लिए बनाया गया*

</div>

---

##  What is DevMentor?

DevMentor is a gamified, AI-powered coding education platform designed specifically for Indian developers. It bridges the gap between generic global platforms and the real needs of India's developer community — with multilingual support, locally relevant examples (UPI, Razorpay, GST), career guidance tailored to Indian companies, and a live community feed.

Everything runs in a **single `index.html` file** — zero build step, zero dependencies to install.

---

## 📸 Pages & Features

###  Dashboard
- Personalized hero section with XP progress, daily streak counter, and level display
- **4-column stat grid**: XP earned, coding streak, problems solved, community rank
- **6 Learning Paths**: Full Stack, AI/ML, Cloud & DevOps, Android, Startup Engineering, DSA & Interview Prep
- Live activity feed, quick-action shortcuts, and a leaderboard sidebar
- Daily challenge countdown timer with XP rewards

###  AI Mentor (`/mentor`)
- Real-time chat interface powered by **Groq's LLaMA 3.3-70b**
- Ask questions in **10 Indian languages**: Hindi, Tamil, Telugu, Bengali, Marathi, Gujarati, Kannada, Malayalam, Punjabi, and English
- Pre-built quick-prompt chips for common developer questions
- Voice input button (UI-ready)
- India-specific context: UPI integrations, startup ecosystem, Indian company interview prep

###  Code Review (`/review`)
- Paste any code snippet and get an AI-powered review
- Pre-loaded sample: a real Razorpay/UPI Python integration with a deliberate security bug
- Structured feedback: bugs, security issues, performance, best practices, suggested fixes
- Simulated review history panel with timestamps

###  Learn (`/learn`)
- **Skill Galaxy** — an interactive visual node graph of skills to unlock
- Module list for each learning path with progress tracking
- Curated video tutorials (free resources)
- Reading list with estimated durations

###  Career (`/career`)
- Role-based roadmaps: SDE-1 → SDE-2 → Senior → Staff
- Company-specific interview prep for **16 Indian & global companies** (Razorpay, Flipkart, Zomato, CRED, Google India, etc.)
- Salary benchmarks for the Indian market
- Resume tips and mock interview mode

###  Community (`/community`)
- Posts feed with category filters: Career, AWS, Startup, Open Source, Tutorial, Questions, Hiring, Showcase
- Like, comment, and bookmark interactions
- **Write a Post modal** with AI-suggested title generation
- Trending tags sidebar
- Active cities leaderboard (Bangalore, Mumbai, Delhi, Chennai, Hyderabad, Pune)
- Event promo widget (e.g., AWS AI for Bharat)

---

##  Gamification System

| Element | Description |
|---|---|
| **XP Points** | Earned by completing modules, code reviews, streaks, and posting |
| **Daily Streak** | Consecutive days of activity, shown in the navbar with  |
| **Levels** | XP thresholds unlock new badges and paths |
| **Achievements** | Badges like First Commit, 14-Day Streak, Speed Coder, Deep Thinker |
| **Leaderboard** | Real-time rank among Indian developers by city |
| **Confetti** | Fires on milestone completions for dopamine hits  |
| **Toast Notifications** | XP gain toasts with slide-up animations |

---

##  Multilingual Support

DevMentor supports **10 Indian languages** selectable from the navbar:

`English` · `हिन्दी` · `தமிழ்` · `తెలుగు` · `বাংলা` · `मराठी` · `ગુજરાતી` · `ಕನ್ನಡ` · `മലയാളം` · `ਪੰਜਾਬੀ`

The AI Mentor responds in whichever language the user selects, making coding education accessible to non-English-first developers across India.

---

## Tech Stack

| Layer | Technology |
|---|---|
| **UI Framework** | React 18 (via CDN, no build step) |
| **JSX Transpilation** | Babel Standalone |
| **AI / LLM** | Groq API — LLaMA 3.3-70b-versatile |
| **Cloud AI** | AWS Bedrock (Claude integration) |
| **Fonts** | Outfit (UI), IBM Plex Mono (code), Noto Sans Devanagari (Indian scripts) |
| **Styling** | Pure CSS with CSS custom properties (no framework) |
| **Deployment** | Single static HTML file |

---

## Getting Started

No installation, no build tools, no `npm install`.

### Try it live
**[https://dev-mentor-s3.s3.eu-north-1.amazonaws.com/index.html](https://dev-mentor-s3.s3.eu-north-1.amazonaws.com/index.html)**



Link = https://dev-mentor-s3.s3.eu-north-1.amazonaws.com/index.html

### Option 1 — Open Directly
```bash
# Just open the file in your browser
open index.html
```

### Option 2 — Serve Locally
```bash
# Using Python
python3 -m http.server 3000

# Using Node.js
npx serve .
```

### Option 3 — Deploy to GitHub Pages / Netlify / Vercel
Drop `index.html` into your repo root and point the deployment to it. Done.

---

## Project Structure

```
devmentor/
└── index.html          # Entire application — HTML + CSS + React JSX
```
---

## Design System

The UI uses a dark-mode-first design with a consistent token system:

```css
--orange:   #f97316   /* Primary CTA, streaks */
--teal:     #14b8a6   /* XP, progress, active states */
--violet:   #8b5cf6   /* AI/ML path, gradients */
--surface-1 … surface-4    /* Layered dark backgrounds */
```

Animated background glow blobs (orange, teal, violet) drift subtly behind all pages for depth, with a dot-grid overlay for texture.

---

## 🛣️ Learning Paths

| Path | Topics | Color |
|---|---|---|
|  Full Stack Dev | React · Node · AWS | Orange |
|  AI & Machine Learning | Python · TensorFlow · Bedrock | Violet |
|  Cloud & DevOps | AWS · Kubernetes · Terraform | Teal |
|  Android Dev | Kotlin · Jetpack Compose | Red |
|  Startup Engineering | UPI · MVP · Scale · GST | Yellow |
|  DSA & Interview Prep | LeetCode · System Design | Green |

Each path has **8 modules** with XP rewards and progress tracking.

---

##  License

MIT License — free to use, modify, and distribute. See [LICENSE](LICENSE) for details.

---

<div align="center">

**DevMentor** · AI for Bharat Hackathon + AWS Bedrock


</div>
