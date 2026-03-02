# 🔤 Wordsearch DE

A German vocabulary word search game playable in the browser. Words are loaded dynamically from a `words.txt` file, with 15 words selected per round across six CEFR proficiency levels.

🔗 **Live Demo:** [kjchiodo.github.io/wordsearch-de](https://kjchiodo.github.io/wordsearch-de/)

---

## Features

- 🇩🇪 German vocabulary organized by CEFR level (A1 → C2)
- 📄 Words loaded from an external `words.txt` file — easy to update without touching code
- 🎯 15 words per round, randomly selected from the chosen level
- 🔁 "New Round" button to regenerate the puzzle
- 📊 Tracks words found and total words per round

---

## CEFR Levels

| Level | Description |
|-------|-------------|
| A1 | Beginner |
| A2 | Elementary |
| B1 | Intermediate |
| B2 | Upper Intermediate |
| C1 | Advanced |
| C2 | Mastery |

---

## words.txt Format

Words are read from a `words.txt` file at the root of the project. The expected format groups words by level:

```
A1
HAUS A1
HUND A1
KATZE A1
...

A2
...
```

To add or update vocabulary, simply edit `words.txt` — no code changes needed.

---

## Getting Started

### Play Online
Visit the live site: [kjchiodo.github.io/wordsearch-de](https://kjchiodo.github.io/wordsearch-de/)

### Run Locally

```bash
git clone https://github.com/kjchiodo/wordsearch-de.git
cd wordsearch-de
# Serve with any static file server, e.g.:
npx serve .
# or
python3 -m http.server
```

> ⚠️ A local server is required because the game fetches `words.txt` via HTTP. Opening `index.html` directly as a file may cause CORS errors.

---

## Project Structure

```
wordsearch-de/
├── index.html       # Main game page
├── words.txt        # German vocabulary by CEFR level
└── ...              # JS/CSS assets
```

---

## Contributing

Have German vocabulary suggestions? Feel free to open a PR with additions to `words.txt`!

---

## License

MIT
