# 🎯 Number Quest — Number Guessing Game

<div align="center">

![Number Quest Banner](https://img.shields.io/badge/Number%20Quest-Mind%20Game-8b5cf6?style=for-the-badge&logo=gamepad&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222222?style=for-the-badge&logo=github&logoColor=white)

**Can you read the computer's mind? 🤔**

A beautiful, interactive number guessing game with Higher/Lower hints, dynamic scoring, and a stunning dark UI.

[🕹️ Play Live](#) • [🚀 Features](#features) • [⚙️ Installation](#installation)

</div>

---

## ✨ Features

- 🎮 **3 Difficulty Levels** — Easy (1–50), Medium (1–100), Hard (1–200)
- 📈 **Higher / Lower Hints** — Color-coded feedback after every guess
- 🔢 **Dynamic Range Narrowing** — Range updates live based on your guesses
- 📊 **Attempts Progress Bar** — Visual bar that turns red as attempts run out
- 🏷️ **Guess History Chips** — See all your previous guesses at a glance
- 🏆 **Scoring System** — Fewer guesses = higher score
- 🎊 **Confetti Animation** — Celebrate when you win!
- 💾 **Local Scoreboard** — Top 5 scores saved in your browser
- 📱 **Fully Responsive** — Works on mobile, tablet, and desktop
- ⌨️ **Keyboard Support** — Press Enter to submit your guess
- 🌌 **Animated Star Background** — Twinkling stars for immersive atmosphere

---

## 🎮 How to Play

1. **Choose a difficulty** — Easy, Medium, or Hard
2. **Enter your guess** in the input box
3. After each guess, you'll receive a hint:
   - 📈 **HIGHER** (cyan) — your guess is too low, go higher!
   - 📉 **LOWER** (pink) — your guess is too high, go lower!
   - 🎉 **CORRECT** (green) — you found the number!
4. **Win** before you run out of attempts to earn points
5. **Score more** by guessing in fewer attempts

### 🏅 Difficulty Details

| Difficulty | Range  | Max Attempts | Base Score |
|------------|--------|--------------|------------|
| 🌱 Easy    | 1–50   | 10 attempts  | 500 pts    |
| 🔥 Medium  | 1–100  | 8 attempts   | 1000 pts   |
| 💀 Hard    | 1–200  | 7 attempts   | 2000 pts   |

---

## 🚀 Installation

### Option 1 — Play Directly (No Setup)

Just open the `index.html` file in any browser. No server, no dependencies needed!

```bash
# Clone the repository
git clone https://github.com/your-username/number-quest-game.git

# Navigate into the folder
cd number-quest-game

# Open in browser
open index.html         # macOS
start index.html        # Windows
xdg-open index.html     # Linux
```

### Option 2 — GitHub Pages (Free Hosting)

1. Fork or clone this repository
2. Go to your repo → **Settings** → **Pages**
3. Under *Branch*, select `main` → click **Save**
4. Your game will be live at:

```
https://your-username.github.io/number-quest-game
```

---

## 📁 Project Structure

```
number-quest-game/
│
├── index.html       # Main game file (HTML + CSS + JS — all in one)
└── README.md        # Project documentation (you are here!)
```

> This project is intentionally kept as a **single HTML file** — making it easy to share, deploy, and host anywhere without any build tools.

---

## 🛠️ Built With

| Technology | Purpose |
|------------|---------|
| **HTML5** | Game structure and layout |
| **CSS3** | Animations, gradients, responsive design |
| **Vanilla JavaScript** | Game logic, scoring, localStorage |
| **Google Fonts** | Outfit + Space Mono typography |

No frameworks. No dependencies. No build step. Just pure HTML/CSS/JS. ✅

---

## 🧠 Game Logic

```
1. Computer picks a random number within the chosen range
2. Player guesses a number
3. If guess < secret → hint: "Go HIGHER"
       range low boundary = guess + 1
4. If guess > secret → hint: "Go LOWER"
       range high boundary = guess - 1
5. If guess == secret → Player WINS 🎉
6. If attempts run out → Game OVER 💔

Score = max(50, baseScore - (attemptsUsed - 1) × (baseScore / maxAttempts))
```

---

## 🔧 Customization

Want to tweak the game? Open `index.html` and find this section in the `<script>` tag:

```javascript
const DIFFICULTIES = {
  easy:   { max: 50,  attempts: 10, scoreBase: 500  },
  medium: { max: 100, attempts: 8,  scoreBase: 1000 },
  hard:   { max: 200, attempts: 7,  scoreBase: 2000 }
};
```

Change `max` to adjust the number range, `attempts` for guesses allowed, and `scoreBase` for points.

---

## 🤝 Contributing

Contributions are welcome! Here's how:

1. **Fork** the repository
2. Create a new branch: `git checkout -b feature/your-feature-name`
3. Make your changes and **commit**: `git commit -m "Add: your feature"`
4. **Push** to your branch: `git push origin feature/your-feature-name`
5. Open a **Pull Request**

### 💡 Ideas for Contribution

- [ ] Add sound effects on hints and win
- [ ] Add a timer mode
- [ ] Multiplayer mode (two players guessing)
- [ ] Dark / Light theme toggle
- [ ] More difficulty levels (Extreme: 1–500)
- [ ] Animated number reveal on game over

---

## 📜 License

This project is open source and available under the [MIT License](LICENSE).

```
MIT License — free to use, modify, and distribute.
Just give credit where it's due! 🙏
```

---

## 👨‍💻 Author

Made with ❤️ by **Divya Guttula**

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/your-username)

---

<div align="center">

**⭐ If you liked this project, please give it a star on GitHub! It means a lot. ⭐**

</div>
