# ⚡ HabitFlow — Personal Habit & Daily Goal Tracker

A minimalist, powerful personal habit and daily goal tracker built as a **zero-dependency, single-file web application** (HTML, CSS, JavaScript in one file, no backend needed). Works 100% offline and in all modern desktop and mobile browsers.

---

## ✨ Features

### 1. 📅 Interactive Tracker Table
- **Dynamic Full-Month Grid**: Automatically computes accurate days of the month (28–31 days, including leap years) with day-of-week headers.
- **Sticky Layout**: Sticky header row and sticky first column (habit name & controls) for smooth horizontal scrolling on mobile and small screens.
- **Today Highlight**: Distinct highlight for today's column with an active `TODAY` pill.
- **Dual Target Types**:
  - **Simple Tick**: Clickable checkbox with micro spring animation.
  - **Numeric Target** (e.g. *Water: 8 glasses*, *Read: 10 pages*): Real-time fractional progress (e.g. `5/8`), completion badge when target is reached, and a stepper dialog (`+`, `−`, `Mark Target`).
- **Month Navigation**: Easily navigate past and future months (`<`, `>`), or jump to today with one click.
- **Row & Column Completion Stats**: Live Done count and % completion for each habit and for every day of the month.

### 2. 🎯 Modifiable Habits & Goals
- **Add & Edit**: Customize habit name, optional category tags, emoji icon presets, and curated color swatches.
- **Reordering**: Move Up (`▲`) and Move Down (`▼`) buttons to organize your routine.
- **Category Filter**: Filter habits by tag (e.g. *Health*, *Fitness*, *Learning*, *Wellness*).
- **Safe Deletion**: Confirmation modal to avoid accidental loss of data.

### 3. 📊 Real-Time Analytics (Chart.js)
- **Daily Momentum (Last 7 Days)**: Bar chart showing percentage of habits completed per day with a rolling 7-day average.
- **Weekly Breakdown**: Performance across weeks of the active month with **Best Week** (emerald) and **Lowest Week** (coral) highlighted automatically.
- **Annual Trend**: 12-month year-at-a-glance line chart with smooth bezier curves and area fill.
- **Habit Comparison**: Horizontal bar chart comparing completion % of each habit for the active month using their assigned colors.
- **Live Reactivity**: Every chart updates instantly the moment you toggle or update any entry.

### 4. 🏆 Streak Tracking & Key Metrics
- **Current Active Streak**: Consecutive completed days leading up to today (keeps streak active if today is still in progress).
- **Longest All-Time Streak**: Historical maximum streak calculation.
- **Summary Cards**: At-a-glance KPIs for *Today's Progress*, *This Week*, *Current Month*, and *Top Active Streak*.
- **Celebration Confetti**: Pure canvas confetti burst when completing all habits for the day.

### 5. 💾 Privacy-First Storage & Portability
- **100% Local**: All data is stored locally in `localStorage` using safe `try/catch` fallbacks. No tracking, no backend, no logins required.
- **Export & Import**: Download your entire history as a JSON backup file (`habitflow-backup-YYYY-MM-DD.json`) and restore it on any device.
- **Clean Reset**: Reset back to fresh sample data with confirmation.
- **Dark & Light Mode**: Built-in sleek dark mode and clean light mode toggle.

---

## 🚀 Quick Start

### Running Locally
No installation or build steps required! Simply clone the repository and open `index.html` in your browser:

```bash
# Clone the repository
git clone https://github.com/atharvtrivedi86-bit/habit-tracker.git

# Open index.html in your default browser (macOS / Linux / Windows)
# Windows:
start index.html
# macOS:
open index.html
# Linux:
xdg-open index.html
```

Or serve locally with any static HTTP server:
```bash
npx serve .
# or
python -m http.server 8000
```

---

## 🌐 Deploy to GitHub Pages (1-Click)

Because HabitFlow is a self-contained static website (`index.html`), you can host it for free on GitHub Pages:

1. Go to your repository on GitHub: `https://github.com/atharvtrivedi86-bit/habit-tracker`
2. Click **Settings** > **Pages** (in the left sidebar).
3. Under **Branch**, select `main` and root `/ (root)`.
4. Click **Save**.
5. Your habit tracker will be live at:
   ```text
   https://atharvtrivedi86-bit.github.io/habit-tracker/
   ```

---

## 🛠️ Tech Stack
- **HTML5 & CSS3**: Custom CSS variables, responsive CSS Grid / Flexbox, sticky tables, and micro-animations.
- **Vanilla JavaScript (ES6+)**: Zero external framework dependencies.
- **Chart.js (v4 via CDN)**: Responsive canvas charts with theme-adaptive styling.
- **Google Fonts**: Plus Jakarta Sans & JetBrains Mono.

---

## 📄 License
MIT License. Free to use, modify, and distribute.