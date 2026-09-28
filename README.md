# VoiceToText Mobile

The iPhone version of [VoiceToText](https://github.com/ArturFeoktystov/VoiceToText): a web app you
add to the home screen. Hold **Dictate**, speak, release → corrected text (Groq Whisper → Claude
Haiku). Hold **Ask** → an answer (Claude Opus). Then **Copy** or **Share** it into any app.

No App Store, no signing, no server. This repository contains **no API keys**: each user types
their own Groq and Anthropic keys in the app's Settings, and they are stored only in that phone's
browser storage.

## Install on iPhone

1. Open the app's GitHub Pages address in **Safari**.
2. Tap **Share** → **Add to Home Screen** → **Add**.
3. Open it from the home screen, tap **⚙︎**, paste your Groq key (`gsk_…`) and Anthropic key
   (`sk-ant-…`), tap **Save**.
4. Hold **Dictate**; allow the microphone the first time.

Keys entered in Safari and in the home-screen app are stored separately — enter them in the
home-screen app.

## Files

| File | What it is |
|---|---|
| `index.html`, `style.css` | The screen |
| `app.js` | Recording, sound bars, Groq + Claude calls, history, settings |
| `manifest.webmanifest`, `icons/` | Home-screen name and icon |
