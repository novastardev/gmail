# gmail

A small, static prank/demo site mimicking a Google-style sign-in flow that transitions into a playful "love letter" page. This repository contains two HTML pages (index.html and love_letter.html) built with plain HTML, CSS and vanilla JavaScript.

> If you enjoyed this little demo, please give this repository a star ⭐ — it really helps!

Important: This project is for novelty/demo purposes only. Do NOT use it to impersonate real services, collect credentials, or engage in phishing. See the Security & Ethics section below.

## Table of contents
- About
- Files in this repo
- Demo / Preview
- Requirements
- Run locally
- How it works
- Customization
- Development & testing
- Security & ethics (must read)
- Contributing
- License
- Author / Contact

## About
This repo contains a simple static UI that imitates a Google sign-in page as a light-hearted prank. When the form is submitted, the UI shows a modal and — if the user confirms — redirects to a "love letter" page. The project is implemented with plain HTML/CSS/JS and requires no build tools.

## Files in this repo
- `index.html` — Main page that mimics a Google-signin UI, with multi-language strings and the interactive prank logic.
- `love_letter.html` — The target page shown when the user confirms; a stylized "confession" with a WhatsApp reply link.
- `README.md` — This file.

There are no build scripts or server-side components in this repository.

## Demo / Preview
- Open `index.html` in a modern browser to view the UI.
- Submitting the password form opens a modal. Pressing "Yes" navigates to `love_letter.html`.

## Requirements
- A modern web browser (Chrome, Firefox, Edge, Safari).
- No back-end or external build required.

## Run locally
Option A — Open file
- On most OSes you can double-click `index.html` to open it in the browser.

Option B — Simple local server (recommended for best behavior)
- Python 3:
  - `cd` into the repository folder
  - `python -m http.server 8000`
  - Open http://localhost:8000/index.html
- Node (http-server):
  - `npm install -g http-server`
  - `http-server -p 8000`
  - Open http://localhost:8000/index.html

## How it works (short)
- `index.html` contains localized strings (translations object) and UI behavior:
  - A faux sign-in form with password input toggling.
  - Localized UI text toggles via the language menu.
  - Submitting the form displays a modal; clicking "Yes" redirects to `love_letter.html`.
  - The "No" button animates away and changes the "Yes" button label.
- `love_letter.html` contains the static letter, a WhatsApp reply link, and decorative animations.

## Customization
- Replace the displayed email and WhatsApp phone/URL in the HTML files before publishing.
- Update the translations object in `index.html` to add or modify languages or phrasing.
- Replace images or assets and add them to an `/assets` folder if desired.
- If you intend to publish screenshots in this README, add images into `/assets` and reference them here.

## Development & testing
- No build steps required. Edit HTML/CSS/JS locally and refresh the browser.
- For cross-browser checks test in Chrome, Firefox, and Safari.
- If you add JS modules or a packaging tool, include a `package.json` and update this README accordingly.

## Security & ethics (MUST READ)
- This repo contains pages that visually imitate a real Google sign-in. Use only for harmless pranks between consenting people, design demos, or learning purposes.
- Do NOT deploy or share versions that can be used to trick people into entering real credentials.
- Never collect, store, or transmit any real user passwords or personal data through this project.
- If you plan to publish the project publicly, explicitly state in the UI and README that it is a demo/prank and not affiliated with Google.
- If you find security-sensitive content (e.g., real credentials) committed in this repo, remove them immediately and rotate the compromised credentials.

## Contributing
Contributions welcome for accessibility improvements, translations, or cleanup.
Please:
1. Fork the repo
2. Create a branch: `git checkout -b feat/my-change`
3. Submit a PR with a clear description of changes and testing steps

Keep changes client-side only (no credential collection).

## Suggested License
MIT License is recommended for permissive open-source usage. If you'd like, I can add a `LICENSE` file with your chosen license.

### Example MIT header (to include in LICENSE):
MIT License
Copyright (c) 2026 novastardev

## Contact / Author
- novastardev — https://github.com/novastardev
- For questions or bug reports, open an issue in this repository.

## Notes before publishing
- Replace any real email addresses, phone numbers, or personal contact links with placeholders or clearly labeled demo values.
- Add a Project description and topic tags on GitHub to clarify that this is a demo/prank and not affiliated with Google.
