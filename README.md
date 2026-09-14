# 🎂 Birthday Card Generator

![HTML5](https://img.shields.io/badge/HTML5-Static_App-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-Animations-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

An interactive birthday card experience built as a single-page static web application. Enter a recipient's name and age, then reveal a personalized animated card with a randomized visual theme, background music, sound effects, confetti, and a downloadable PNG version.

## 🌐 Live Demo

**[Open the Birthday Card Generator](https://ichigosky21.github.io/birthday-gift/)**

## ✨ Features

- **Personalized greeting** — Generates the birthday card from the recipient's name and age.
- **Five randomized themes** — Teal & Gold, Purple Dream, Midnight Rose, Forest Glow, and Sunset Blaze.
- **Interactive door sequence** — Unlock the card through an animated door-and-key interaction.
- **Age-based badge** — Displays the recipient's age as a medal-style badge.
- **Dynamic celebration effects** — Confetti and floating birthday-themed emojis are generated during the experience.
- **Birthday message** — Includes a personalized greeting and Korean birthday phrase (`생일 축하해!`).
- **Background music player** — Randomly selects one bundled track and provides play/pause, progress, and seeking controls.
- **Web Audio UI sounds** — Generates short interaction sounds with the Web Audio API instead of additional sound-effect files.
- **Save as PNG** — Uses `html2canvas` to capture the generated card as an image.
- **Responsive interface** — Designed for both desktop and mobile screens.
- **Keyboard-friendly controls** — Interactive controls include keyboard handling and ARIA labels in the interface.

## 🎬 User Flow

```text
Enter name & age
       ↓
Create personalized card
       ↓
Random theme + music selected
       ↓
Unlock the animated door
       ↓
Birthday badge + celebration effects
       ↓
Reveal the birthday message
       ↓
Play music or save the card as PNG
```

## 🎨 Visual Themes

The application currently contains five themes. Each theme changes the accent, background, metallic badge, and door colors:

| Theme | Style |
|---|---|
| **Teal & Gold** | Teal background with warm gold accents |
| **Purple Dream** | Purple gradient with bright pink/violet accents |
| **Midnight Rose** | Dark blue palette with rose highlights |
| **Forest Glow** | Deep green palette with lime/cyan accents |
| **Sunset Blaze** | Indigo background with orange/coral accents |

A theme is selected randomly when the card is created.

## 🎵 Background Music

The current playlist contains four bundled audio files:

| Track | Artist | Starting Position |
|---|---|---:|
| Monokrom | Tulus | 0:30 |
| Just The Way You Are | Bruno Mars | 0:15 |
| OMG | NewJeans | 0:40 |
| APT | ROSÉ & Bruno Mars | 0:00 |

The application randomly selects a track when a new card is generated. Music playback starts from the configured position after the interactive door is opened, subject to browser autoplay policies.

> **Important:** The repository contains copies of commercially released music tracks. If you redistribute, deploy, or modify this project publicly, make sure you have the necessary rights or permissions for any bundled audio assets. The repository currently does not include a separate `LICENSE` file for the project or the audio files.

## 🖼️ Saving the Card

After the birthday message is revealed, the **Save as Image** action captures the card using `html2canvas` and generates a PNG file named using the recipient's name.

Because `html2canvas` is loaded from jsDelivr, an internet connection may be required for the image-export feature if the library has not already been cached by the browser.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Application structure and semantic markup |
| CSS3 | Layout, responsive styling, themes, glassmorphism, and animations |
| Vanilla JavaScript | Application logic, personalization, randomization, audio controls, and interactions |
| Web Audio API | Short UI sound effects |
| html2canvas 1.4.1 | Client-side PNG capture |
| Google Fonts | Fredoka and Karla typefaces |

There is **no package manager or build step**. The application is designed to run directly as a static website.

## 📁 Project Structure

```text
birthday-gift/
├── index.html          # Complete application: HTML, CSS, and JavaScript
├── monokrom.mp3        # Bundled background track
├── jtwya.mp3           # Bundled background track
├── omg.mp3             # Bundled background track
├── apt.mp3             # Bundled background track
└── README.md           # Project documentation
```

## 🚀 Running Locally

Clone the repository:

```bash
git clone https://github.com/IchigoSky21/birthday-gift.git
cd birthday-gift
```

Then open `index.html` in a modern browser.

For the most reliable behavior—especially when testing external CDN resources—serve the directory through a local HTTP server instead of relying on a `file://` URL.

For example, with Python:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000` in your browser.

## 🎵 Adding or Replacing Music

The playlist is defined directly in `index.html`:

```javascript
const PLAYLIST = [
  { file: 'monokrom.mp3', title: 'Monokrom', artist: 'Tulus', startAt: 30 },
  { file: 'your-song.mp3', title: 'Your Song', artist: 'Artist Name', startAt: 0 }
];
```

Place the corresponding audio file next to `index.html`, then add it to the `PLAYLIST` array.

For public redistribution, prefer music that you have permission to use or that is available under an appropriate license.

## ♿ Accessibility & Compatibility

The interface includes keyboard interactions for key and music controls, ARIA labels for relevant interactive elements, and responsive layouts for smaller screens.

The project targets modern desktop and mobile browsers with support for standard HTML5, CSS3, JavaScript, Web Audio API, and client-side canvas rendering.

## 📌 Current Limitations

- The application is intentionally a static, client-side experience; there is no backend, database, or user account system.
- Background music depends on the bundled audio assets and browser media policies.
- The PNG export depends on the `html2canvas` CDN resource being available.
- The project currently bundles copyrighted commercial music tracks; redistribution rights should be verified before public reuse.
- The generated birthday message is fixed in the application logic apart from the recipient's name and age.
- The project does not currently include an open-source license file.

## 🤝 Contributing

Contributions and improvements are welcome.

1. Fork the repository.
2. Create a feature branch:

   ```bash
   git checkout -b feature/your-feature
   ```

3. Make and test your changes.
4. Commit your changes.
5. Push the branch and open a pull request.

When contributing, please keep the project lightweight and preserve its static, dependency-free architecture where practical.

## 📄 License

No `LICENSE` file is currently included in this repository. Until a license is explicitly added, do not assume that the source code or bundled media is freely licensed for redistribution.

---

<div align="center">

**Made with ❤️ by [IchigoSky21](https://github.com/IchigoSky21)**

🎂 *A small interactive way to make someone's birthday a little more memorable.* 🎂

</div>
