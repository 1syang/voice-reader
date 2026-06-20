# Voice Reader

A browser-based text-to-speech reader that supports PDF, DOCX, EPUB, web URLs, and pasted text. No installation or server required — open `index.html` in Chrome or Edge and start reading.

## Features

- **Multiple input formats** — PDF, DOCX (Word), EPUB, any public web URL, or paste/type text directly
- **Natural voices** — uses the Web Speech API with all available system voices (English voices listed first)
- **Sentence highlighting** — highlights and scrolls to the current sentence as it reads
- **Playback controls** — Play, Pause/Resume, Stop; click any sentence to jump to it
- **Rate & pitch sliders** — tune the voice to your preference
- **No dependencies to install** — all libraries loaded from CDN

## Usage

1. Open `index.html` in Chrome or Edge
2. Choose an input method (File / URL / Paste)
3. Select a voice and adjust rate/pitch if desired
4. Click **Play**

### Best voices by platform

- **Windows** — Microsoft Aria or Microsoft Jenny (if available) are significantly more natural than older voices
- **macOS** — Samantha or Alex work well; Siri voices are best if enabled in System Preferences
- **Chrome on any platform** — Google voices (marked "Google" in the voice list) are generally high quality

### URL loading

The URL tab fetches pages via [allorigins.win](https://allorigins.win) as a CORS proxy. Most public web pages work; paywalled or login-required pages will not.

## Deployment

This is a single static HTML file — it can be hosted anywhere that serves static files.

**GitHub Pages:**
1. Upload `index.html` to a GitHub repository
2. Go to Settings → Pages → Deploy from branch → `main` / `/ (root)`
3. Site will be live at `https://yourusername.github.io/your-repo/`

## Libraries Used

- [PDF.js](https://mozilla.github.io/pdf.js/) — Mozilla, Apache 2.0
- [mammoth.js](https://github.com/mwilliamson/mammoth.js) — Michael Williamson, BSD 2-Clause
- [JSZip](https://stuk.github.io/jszip/) — Stuart Knightley, MIT

## License

Apache License 2.0 — see [LICENSE](LICENSE) for details.
