# gmail

A small, static prank/demo site mimicking a Google-style sign-in flow that transitions into a playful "love letter" page. Built with plain HTML, CSS and vanilla JavaScript — no build tools, no backend.

> If you enjoyed this little demo, please give this repository a star ⭐ — it really helps!

**Important:** This project is for novelty/demo purposes only. Do NOT use it to impersonate real services, collect credentials, or engage in phishing. See the [Security & ethics](#security--ethics-must-read) section below.

## Table of contents
- [About](#about)
- [Files in this repo](#files-in-this-repo)
- [Run locally](#run-locally)
- [How it works](#how-it-works)
- [Customization](#customization)
- [Security & ethics](#security--ethics-must-read)
- [Contributing](#contributing)
- [License](#license)
- [Author](#author)

## About
A simple static UI that imitates a Google sign-in page as a light-hearted prank. When the form is submitted, the UI shows a modal and — if the user confirms — redirects to a "love letter" page.

## Files in this repo
- `index.html` — Main page that mimics a Google sign-in UI, with multi-language strings and the interactive prank logic.
- `love_letter.html` — The target page shown when the user confirms; a stylized "confession" with a WhatsApp reply link.

## Run locally
**Option A — open the file:** double-click `index.html` in a modern browser (Chrome, Firefox, Edge, Safari).

**Option B — local server (recommended):**
```bash
python -m http.server 8000
# open http://localhost:8000/index.html
```

## How it works
- `index.html` contains a translations object and UI behavior:
  - A faux sign-in form with password input toggling.
  - Localized UI text toggles via the language menu.
  - Submitting the form displays a modal; clicking "Yes" redirects to `love_letter.html`.
  - The "No" button animates away and changes the "Yes" button label.
- `love_letter.html` contains the letter, a WhatsApp reply link, and decorative animations.

## Customization
- Replace the displayed email and WhatsApp link in the HTML files with your own (demo) values.
- Update the translations object in `index.html` to add languages or phrasing.
- Add screenshots to an `/assets` folder if you want them in this README.

## Security & ethics (must read)
- These pages visually imitate a real Google sign-in. Use only for harmless pranks between consenting people, design demos, or learning purposes.
- Do NOT deploy or share versions that can be used to trick people into entering real credentials.
- Never collect, store, or transmit any real user passwords or personal data through this project.
- Not affiliated with, endorsed by, or connected to Google in any way.

## Contributing
Contributions welcome for accessibility improvements, translations, or cleanup:

1. Fork the repo
2. Create a branch: `git checkout -b feat/my-change`
3. Submit a PR with a clear description

Keep changes client-side only (no credential collection).

## License
Released under the [MIT License](LICENSE).

## Author
**novastardev** — https://github.com/novastardev

For questions or bug reports, open an issue in this repository.
