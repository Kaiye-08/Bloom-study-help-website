# 🌱 Bloom

**Study until you flower.** Bloom is a gamified study website where a little flowering plant grows with every right answer and wilts with every wrong one. Make your own quizzes, survive revenge rounds, take movement breaks, and treat yourself when you earn it.

Built with plain HTML, CSS, and JavaScript in a single file. No framework, no build step, no backend.

<!-- Add a screenshot or GIF here: ![Bloom demo](demo.gif) -->

## ✨ Features

**Study loop**
- **Plant mascot:** moves through withered, wilting, budding, unfurling, and full bloom depending on how you do. Get answers wrong for long enough and it dies.
- **Hearts and streaks:** a wrong answer costs a heart and resets your streak, with a "BONK!" animation and sound.
- **Revenge rounds:** missed questions come back a couple of questions later. Win one to earn a heart back and bonus XP.
- **Difficulty modes:** Chill, Normal, and Hardcore change your hearts and how fast the plant wilts.
- **Multiple choice or typed answers:** add wrong options for multiple choice, or leave them blank to type the answer from memory.

**Focus and wellbeing**
- **Movement quests:** every 5 answers you get a 30-second timer (jumping jacks, a walk, stretching, deep breaths) for bonus XP and a plant boost.
- **Focus sound:** brown noise, white noise, or binaural beats, all generated in the browser with the Web Audio API. Binaural beats need headphones and the research on them is mixed, so treat them as ambiance.

**Rewards and progress**
- **Treat journal:** earn a treat at XP milestones, when you clear all your revenge questions, or when you finish with your plant in full bloom. Pick from your own treat menu and log it with the date and what you did to earn it.
- **Garden:** every finished session plants a mini version of your plant, so you can look back at your blooms (and your withered ones).
- **Home screen:** greeting, latest plant, stats, and a progress bar to your next treat.
- **Reset:** wipe your progress, or erase everything, with a two-tap confirmation.

**Look and feel**
- Five pastel Frutiger Aero themes: Sky, Cotton candy, Mint lagoon, Twilight, and Moonlit pond.
- Glassy cards, glossy buttons, and floating bubbles.

## 🚀 Run it

1. Download `bloom.html`.
2. Open it in any modern browser.

That's it. To host it, upload the file to GitHub Pages, Netlify, or Vercel.

> The page loads the Nunito font from Google Fonts. Without internet it falls back to your system font and everything else still works.

## 💾 Data

Quizzes, XP, garden, treat journal, and your chosen theme are saved in your browser's `localStorage`. Nothing is sent anywhere. Clearing your browser data or switching browsers or devices means starting fresh.

## 🗂 Project structure

```
bloom.html   # the whole app: markup, styles, and scripts
README.md
```

Inside `bloom.html`:
- **Pages:** Home, Quizzes, Create, Garden, Treats, Focus, plus the study screen.
- **Plant:** drawn as inline SVG, generated from a 0 to 100 health value.
- **Sounds:** short oscillator tones for the bonk, chime, and sparkle.
- **Themes:** CSS variables switched with a `data-theme` attribute on the root element.

## 🛣 Roadmap

- [ ] Classical background music (royalty-free recordings only)
- [ ] Scan printed questions with OCR (e.g. Tesseract.js)
- [ ] Shared study squads and friend leaderboards
- [ ] Spaced repetition for missed questions
- [ ] Exam countdown planner
- [ ] Mobile app version

## 🤝 Contributing

Ideas and pull requests are welcome. Open an issue first for bigger changes.

## 📄 License

MIT License
