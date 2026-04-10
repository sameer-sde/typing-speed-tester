# ⌨️ TypeFast — Typing Speed Tester

TypeFast is a sleek, gamified typing speed tester built with plain HTML, CSS, and JavaScript. Practice your typing, chase new personal bests, and track your progress over time — all in the browser.

---

## 🚀 Live Demo

🔗 [View Live Demo](https://sameer-sde.github.io/typing-speed-tester/)

---

## ✨ Features

- ⚡ Real-time stats: WPM, CPM, accuracy, errors, and time left.
- 🕒 Multiple time limits: **15s, 30s, 60s, 120s**.
- 🎮 Practice modes:
  - 📝 Words
  - 🧠 Quotes
  - 🔢 Numbers
  - 💻 Code
  - 🧘 Zen (relaxed, untimed-style behavior)
  - 💀 Sudden Death (one mistake and you’re out)
  - 🙈 Blind (future characters hidden)
- 🎚 Difficulty levels: **Easy**, **Medium**, **Hard** word packs.
- 🎹 On-screen keyboard with key highlights for correct/incorrect presses.
- 🧪 Detailed results screen with breakdown and achievements.
- 🏆 Best WPM tracking and recent tests history.
- 📈 XP, levels, and daily streak tracking.
- 📋 One-click “Copy Score” for sharing your result.
- 📤 CSV export for your typing history.
- 🎨 Light/Dark theme toggle.
- 🔊 Optional sound effects for typing and test completion.
- 🎉 Confetti animation on new personal bests.

---

## 🧱 Tech Stack

- 🌐 **HTML5**
- 🎨 **CSS3** (custom theming + responsive layout)
- 🧠 **Vanilla JavaScript**
- 🔤 **Google Fonts**
  - JetBrains Mono
  - Space Grotesk
- 💾 **localStorage** for user data persistence

---

## 📂 Project Structure

```text
.
├── index.html      # Single-page app with HTML, CSS, and JS
└── README.md       # Project documentation
```

---

## 🚀 How It Works

### 🔄 Core flow

1. Open the app in your browser.
2. Pick **time**, **mode**, and **difficulty**.
3. Start typing in the input box — the test starts on your first keystroke.
4. Press **Space** to commit a word (in normal timed modes).
5. When time is up, a results modal shows your stats and achievements.

### 📊 Stats

During and after a test, you see:

- **WPM** (words per minute, based on committed words)
- **CPM** (characters per minute)
- **Accuracy** (% of correctly typed words)
- **Errors** (total mismatches)
- **Words typed**
- **Best WPM** so far

### 🎮 Modes (Quick Overview)

- **Words** — Shuffled word list based on difficulty.
- **Quotes** — Long quote-style sentences for flow practice.
- **Numbers** — Random numbers up to 4 digits.
- **Code** — JavaScript-like snippets for coding-style typing.
- **Zen** — Relaxed mode that focuses more on live stats than strict timing.
- **Sudden Death** — Any mistake instantly restarts the test.
- **Blind** — Future characters are replaced with bullets for extra challenge.

---

## 🌱 Progression & Persistence

Data stored in `localStorage` (per browser/device):

- `tft_history` — recent tests (date, WPM, accuracy, mode, time, difficulty).
- `tft_best` — best WPM.
- `tft_xp` — total XP.
- `tft_streak` — active daily streak.
- `tft_lastdate` — last day you played.

XP is awarded based on your **speed × accuracy**, which drives:

- Level name (Beginner → Legend)
- Level number
- XP progress bar

---

## 🖥 Installation & Setup

No build step needed — it’s just one HTML file.

1. Save the provided code as `index.html`.
2. Double-click `index.html` or open it via:
   - Right-click → “Open With” → Your browser, or
   - Drag the file into a browser window.
3. Start typing to begin your first test.

---

## 🎛 Usage Tips

- ⏱ Change time: use the **Time** buttons (15s / 30s / 60s / 120s).
- 🧪 Switch mode: use the **Mode** row (Words, Quotes, Numbers, Code, Zen, Sudden Death, Blind).
- 🎚 Change difficulty: **Diff** dropdown (Easy/Medium/Hard).
- 🔠 Adjust font & size: use **Font** dropdowns.
- 🔁 Quick restart: **Tab** (focus must be on the page).
- 📋 Copy latest score: click **“Copy Score”**.
- 📤 Export CSV: click **“Export CSV”** to download your test history.
- 🧹 Clear history: **“Clear History”** button.
- 🌗 Theme: toggle **Dark / Light** from the header.
- 🔊 Sound: toggle **Sound ON/OFF** from the header.

---

## ⌨️ Keyboard Shortcuts

- `Tab` — Restart the test.
- `Space` — Commit the current word (during active tests).

---

## 🧩 UI Highlights

- Character-level highlight: green for correct, red for wrong, with an animated cursor.
- Word-level highlight for the current and incorrect words.
- Live virtual keyboard with green/red key flashes for feedback.
- XP level badge and progress bar in the header.
- Daily streak badge (e.g., 🔥 `5-day streak`).
- Result overlay with:
  - WPM, CPM, Accuracy, Errors, Words, Best WPM
  - Achievement badges (e.g., ⚡ Speed Demon, 🎯 Accuracy King)
  - Friendly AI-style message based on your performance.

---

## 📊 Data Export

Use **Export CSV** to get a `typing_history.csv` file with columns:

- Date  
- WPM  
- Accuracy  
- Mode  
- Difficulty  
- Time  

You can open this in Excel, Google Sheets, or any CSV viewer.

---

## 🌐 Browser Support

Tested or expected to work in modern browsers:

- Chrome
- Edge
- Firefox
- Safari

(localStorage and basic audio APIs are required.)

---

## 💡 Ideas for Future Enhancements

- 👥 Online race / multiplayer mode.
- ☁️ Account system and cloud sync for stats.
- 🌍 Multi-language word lists.
- ✏️ Custom text mode (paste your own text).
- 📈 Progress charts for WPM/accuracy over time.
- 🦾 More detailed per-character accuracy analytics.
- ♿ Extra accessibility and screen reader optimizations.

---

## 📜 License

This project is created for learning and personal use.

If you want to make it open source, add a proper license such as MIT or Apache-2.0 in a `LICENSE` file.
