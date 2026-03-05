# ⏱️ Pomodoro Timer App

A modern, feature-rich Pomodoro Timer built with **React**, **TailwindCSS**, and **Framer Motion**. Stay focused and productive with customizable timers, progress tracking, and theme toggling.

---

## 🔥 Features  
 
✅ **Session / Break Timers**      
✅ **Customizable Durations**     
✅ **Visual Progress Indicator (SVG Circle)**    
✅ **Light / Dark Theme Toggle**   
✅ **Simple Stats Tracking (Completed Sessions)**   
✅ **Daily Goal Tracking**      
✅ **Pomodoro Chart (Daily Stats Visualization)**     
✅ **Desktop Notifications API Support**  
✅ **Smooth Animations via Framer Motion**  
✅ **LocalStorage Persistence**  

---
 
## 📁 Project Structure

```
Directory structure:
└── hariharans24-pomodoro-react-tailwind/
    ├── README.md
    ├── LICENSE
    ├── package.json
    ├── postcss.config.js
    ├── tailwind.config.js
    ├── public/
    │   └── index.html
    └── src/
        ├── App.js
        ├── index.js
        ├── components/
        │   ├── Controls.jsx
        │   ├── PomoChart.jsx
        │   ├── Settings.jsx
        │   ├── Stats.jsx
        │   ├── Tasks.jsx
        │   ├── ThemeToggle.jsx
        │   └── TimerDisplay.jsx
        ├── context/
        │   └── ThemeContext.jsx
        └── styles/
            └── index.css
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/HARIHARANS24/pomodoro-react-tailwind.git
cd pomodoro-react-tailwind
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Run Development Server

```bash
npm run start
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## 📦 Built With

- [React](https://reactjs.org/) — UI framework
- [TailwindCSS](https://tailwindcss.com/) — Utility-first CSS
- [Framer Motion](https://www.framer.com/motion/) — Animation library
- [Lucide React](https://lucide.dev/) — Icons
- [Recharts](https://recharts.org/) — Charting library for Pomodoro stats
- [Vite](https://vitejs.dev/) — Fast dev server and build tool

---

## 🌙 Theming 

Toggle light/dark mode using the 🌙/☀️ button in the top-right corner. The selected theme is persisted using `localStorage`.

---

## ⚙️ Customization

### Modify Timer Durations

You can adjust default durations in `App.jsx`:

```js
const [sessionLength, setSessionLength] = useState(25 * 60); // 25 minutes
const [breakLength, setBreakLength] = useState(5 * 60); // 5 minutes
```

Or use the UI inputs under "Session / Break" settings to adjust on the fly.

---

## 💾 Data Persistence

- **Theme selection** is saved in `localStorage`
- **Completed session count** is stored in `localStorage` under the `completed` key
- **Daily goal** is saved under `dailyGoal`
- **Daily session data** (by date) is stored under `dailyStats`

---

## 📊 Stats & Tracking

### ✅ Completed Sessions

View how many Pomodoro sessions you’ve completed since you began using the app.

### 🎯 Daily Goal Tracking

Set and track a daily goal (e.g. 8 Pomodoros per day). See your progress toward that goal live.

### 📈 Pomo Chart

A bar chart visualizes how many Pomodoros you completed over the last 7 days. Powered by **Recharts**.

---

## 🔔 Notifications API

The app supports browser notifications for:

- ✅ Session complete
- ✅ Break complete

> Make sure to **allow notifications** when prompted by your browser.

---

## ✨ Animations

The timer circle uses smooth stroke transitions, and Framer Motion can animate components like settings, modals, or the stats area.

---

## 🧪 Available Scripts

```bash
npm run dev       # Start development server
npm run build     # Build for production
npm run preview   # Preview production build
```

---

## 🧰 Tailwind Configuration

```js
/** @type {import('tailwindcss').Config} */
export default {
  content: ["./index.html", "./src/**/*.{js,jsx}"],
  darkMode: "class",
  theme: {
    extend: {},
  },
  plugins: [],
};
```

---

## 📌 Requirements

- Node.js ≥ 16
- npm ≥ 7

---


## 🤝 Contributing

Pull requests are welcome! Open an issue first to propose changes, features, or bug fixes.

---

## 📄 License

MIT © [HARIHARANS24](https://github.com/HARIHARANS24/pomodoro-react-tailwind/blob/main/LICENSE)

---

## 🧠 Inspiration

This app follows the **Pomodoro Technique** – a time management method that encourages working in focused intervals (typically 25 minutes) followed by short breaks.

Stay focused, stay sharp! 💡

