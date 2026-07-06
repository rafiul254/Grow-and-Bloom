
#                                    Grow & Bloom — Hand Tracking Flower App 🌸


<div align="center">

![Made with HTML](https://img.shields.io/badge/Made%20with-HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![MediaPipe](https://img.shields.io/badge/MediaPipe-Hands-0097A7?style=for-the-badge&logo=google&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Live-brightgreen?style=for-the-badge)

**A real-time webcam-based hand tracking app where your hands grow and bloom flowers — built with MediaPipe Hands & Canvas API.**

[🌐 Live Demo](https://rafiul254.github.io/Grow-and-Bloom/) · [🐛 Report Bug](../../issues) · [✨ Request Feature](../../issues)

</div>

---

## 📸 Preview
<img width="1600" height="758" alt="WhatsApp Image 2026-07-06 at 12 50 26 PM" src="https://github.com/user-attachments/assets/469d2dde-b8b7-41b0-8e09-438a060af9be" />


> Right hand raised → stem grows 🌱  
> Open your palm → flower blooms 🌸  
> Two hands → two flowers 🌺🌺

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🌱 **Real-time Hand Tracking** | Powered by Google MediaPipe Hands — detects 21 landmarks per hand |
| 🌸 **Two Flowers** | Right hand controls left flower, Left hand controls right flower |
| 🎨 **3 Color Themes** | Rose 🌸 · Sunflower 🌻 · Lotus 🪷 — switch anytime |
| 🎵 **Sound Effects** | Soft chime plays when flowers bloom (Web Audio API) |
| 🌧️ **Petal Rain** | Petals fall from the sky when bloom is at full intensity |
| 🎥 **Cinematic Blur** | Backdrop blur on camera feed for a dreamy look |
| 💡 **Color Enhancement** | Auto brightness, contrast & saturation boost for low-quality cameras |
| 🪴 **Flower Pot** | Beautiful 3D-style clay pot drawn with Canvas gradients |
| ☀️🌙 **Day / Night Mode** | Toggle between light and dark backgrounds |
| ⚙️ **Camera Switcher** | Switch between multiple connected cameras |
| 🪞 **Mirror Toggle** | Flip the camera view on/off |
| 📍 **Landmark Overlay** | Optional hand skeleton visualization |

---

## 🚀 Getting Started

### Prerequisites

- A modern browser: **Google Chrome** or **Microsoft Edge** (recommended)
- A working **webcam**
- **Internet connection** (MediaPipe loads from CDN)

> ⚠️ Firefox may have issues with MediaPipe. Use Chrome/Edge for best experience.

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/grow-and-bloom.git
   ```

2. **Navigate to the folder**
   ```bash
   cd grow-and-bloom
   ```

3. **Open in browser**
   ```bash
   # Simply open the file in Chrome
   open index.html
   # OR double-click index.html in your file explorer
   ```

4. **Allow camera permission** when prompted

> No npm, no build tools, no dependencies to install. Just open and play! 🎉

---

## 🎮 How to Use

```
┌─────────────────────────────────────────────────┐
│                                                 │
│   ✋ RIGHT HAND          🤚 LEFT HAND            │
│                                                 │
│   Raise hand UP    →   Left flower stem grows   │
│   Open palm wide   →   Left flower blooms       │
│                                                 │
│   Raise hand UP    →   Right flower stem grows  │
│   Open palm wide   →   Right flower blooms      │
│                                                 │
└─────────────────────────────────────────────────┘
```

### Controls Summary

| Action | Result |
|--------|--------|
| Raise right hand high | Left stem grows taller |
| Open right palm | Left flower blooms |
| Raise left hand high | Right stem grows taller |
| Open left palm | Right flower blooms |
| Lower your hand | Stem slowly shrinks |
| Close your palm | Flower slowly folds |

### Tips for Best Experience
- 💡 Sit in a **well-lit room** facing a window
- 📏 Keep your hands **within the camera frame**
- 🖐️ Raise hand **above shoulder level** for full stem growth
- 🌸 Spread all 5 fingers wide for maximum bloom
- 🎨 Try switching themes while flowers are blooming!

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **HTML5 Canvas** | Drawing flowers, stems, particles, pot |
| **CSS3** | UI styling, animations, day/night mode |
| **Vanilla JavaScript** | App logic, state management |
| **MediaPipe Hands** | Real-time hand landmark detection |
| **Web Audio API** | Procedural chime sound generation |
| **MediaDevices API** | Webcam access & camera switching |

---

## 📁 Project Structure

```
grow-and-bloom/
│
├── index.html          # Complete app — single file, no dependencies
├── README.md           # Project documentation
└── .gitignore          # Git ignore rules
└── License 
```

> The entire app lives in a **single `index.html` file** — no frameworks, no bundlers, no build step.

---

## 🌐 Deploy to GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings** → **Pages**
3. Under **Source**, select `main` branch → `/ (root)`
4. Click **Save**
5. Your app will be live at:
   ```
   https://your-username.github.io/grow-and-bloom
   ```

---

## 🔧 Customization

You can easily customize the app by editing the `THEMES` object in `index.html`:

```javascript
const THEMES = {
  rose: {
    stemColor: '#16a34a',
    stemGlow: '#22c55e',
    petalHues: [330, 345, 310, 355, 320, 340],
    petalSat: 85,
    petalLight: 68,
    petalEmoji: ['🌸', '💮', '🌺', '🩷'],
    // ... more options
  },
  // Add your own theme here!
  myTheme: {
    stemColor: '#your-color',
    // ...
  }
};
```

---

## 🐛 Known Issues

- MediaPipe may take **5–10 seconds** to load on slow connections
- Camera permissions must be **explicitly allowed** in browser settings
- Works best in **good lighting** — low light causes hand detection issues
- Firefox has limited MediaPipe support — use **Chrome or Edge**

---

## 🤝 Contributing

Contributions are welcome! Here's how:

1. Fork the repository
2. Create a feature branch
   ```bash
   git checkout -b feature/my-new-feature
   ```
3. Commit your changes
   ```bash
   git commit -m "feat: add my new feature"
   ```
4. Push to the branch
   ```bash
   git push origin feature/my-new-feature
   ```
5. Open a **Pull Request**

---

##  Future Ideas

- [ ] More flower types (Cherry Blossom, Orchid)
- [ ] Background scene (garden, night sky)
- [ ] Photo/screenshot capture button
- [ ] Mobile touch support
- [ ] Offline mode (bundle MediaPipe locally)
- [ ] Multiple color petal gradients
- [ ] Wind effect on flowers

---

## 📄 License

This project is licensed under the **MIT License** — feel free to use, modify, and distribute.


---

## 👤 Author

**Rafiul Islam**  
🌐 [your-portfolio.com](https://portfolio-website-rafiul.vercel.app/)  
💼 [LinkedIn](https://www.linkedin.com/in/rafiul-islam-25sep92004)  
🐙 [GitHub](https://github.com/rafiul254)

---

<div align="center">

Made for fun🌸 · If you like this project, give it a ⭐!

</div>
