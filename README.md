# ⏱️ Pomodoro Timer App

A modern, feature-rich Pomodoro Timer built with **React**, **TailwindCSS**, and **Framer Motion**. Stay focused and productive with customizable timers, stats tracking, and theme toggling.

---

## 🔥 Features

✅ **Session / Break Timers**  
✅ **Customizable Durations**  
✅ **Visual Progress Indicator (SVG Circle)**  
✅ **Light / Dark Theme Toggle**  
✅ **Simple Stats Tracking (Completed Sessions)**  
✅ **Smooth Animations via Framer Motion**  
✅ **LocalStorage Persistence**  

---

## 📁 Project Structure

```
pomodoro-app/
├── public/
│   └── index.html
├── src/
│   ├── components/
│   │   ├── TimerDisplay.jsx      // Main timer circle and countdown
│   │   ├── Controls.jsx          // Start/Pause/Reset buttons
│   │   ├── Settings.jsx          // Adjust session/break lengths
│   │   ├── Stats.jsx             // Displays completed session count
│   │   └── ThemeToggle.jsx       // Light/Dark theme switch
│   ├── context/
│   │   └── ThemeContext.jsx      // Theme context logic
│   ├── App.jsx                   // Main app logic and layout
│   ├── main.jsx                  // App entry point
│   └── index.css                 // Tailwind base styles and custom styles
├── tailwind.config.js           // Tailwind setup
├── package.json                 // Project dependencies and scripts
└── vite.config.js               // Vite configuration
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
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) in your browser.

---

## 📦 Built With

- [React](https://reactjs.org/) — UI framework
- [TailwindCSS](https://tailwindcss.com/) — Utility-first CSS
- [Framer Motion](https://www.framer.com/motion/) — Animation library
- [Lucide React](https://lucide.dev/) — Icons
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
- **Completed session count** is also stored in `localStorage` under the `completed` key

---

## 📊 Stats

See how many Pomodoro sessions you've completed with a live counter at the bottom of the app.

---

## ✨ Animations

The timer's SVG circle updates smoothly using CSS transitions, while the rest of the app structure is animation-ready with Framer Motion (you can expand on this for animated settings/stats, etc.).

---

## 🧪 Available Scripts

### Start development server

```bash
npm run dev
```

### Build for production

```bash
npm run build
```

### Preview production build locally

```bash
npm run preview
```

---

## 🧰 Tailwind Configuration

Minimal `tailwind.config.js`:

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

## 📸 Screenshots

> Add screenshots here if needed:
- Light/Dark Mode
- Running Timer
- Settings UI
- Stats Display

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.

---

## 📄 License

MIT © [HARIHARANS24](https://github.com/HARIHARANS24/pomodoro-react-tailwind/blob/main/LICENSE)

---

## 🧠 Inspiration

This app follows the Pomodoro Technique – a time management method that encourages working in focused intervals (typically 25 minutes) followed by short breaks.

Stay focused, stay sharp! 💡
