# ALMEER AI v4.0
### Human-like Autonomous Intelligence · Created by Sydney Sider

---

## Features

- **Human-like personality** — Emotions, empathy, natural speech patterns
- **Voice input** — Speak to ALMEER using your mic (Chrome/Edge)
- **Voice responses** — ElevenLabs TTS or browser TTS fallback
- **App launcher** — Open YouTube, Spotify, GitHub, Maps, Gmail etc by voice or click
- **Device controls** — Camera, location, notifications, fullscreen, clipboard, wake lock
- **Smart commands** — `/search`, `/code`, `/debug`, `/agent`, `/translate`, `/summarize`
- **Voice commands** — "Open YouTube", "Set a timer for 5 minutes", "What time is it?"
- **AI Memory** — Remembers your conversation context
- **Agent mode** — Multi-step autonomous task execution
- **Cyberpunk UI** — Dark red, animated particles, smooth animations

---

## Deploy to Railway (Recommended)

1. **Push to GitHub**
```bash
git init
git add .
git commit -m "ALMEER AI v4"
git remote add origin https://github.com/SIDER44/almeer-ai.git
git push -u origin main
```

2. **Deploy on Railway**
   - Go to [railway.app](https://railway.app) → New Project → Deploy from GitHub
   - Select your repo
   - Go to **Variables** tab and add:

```
ANTHROPIC_API_KEY = sk-ant-your-key-here
CLAUDE_MODEL      = claude-opus-4-5
MAX_TOKENS        = 2048
```

3. **Done!** Railway gives you a live URL instantly.

---

## Run Locally

```bash
npm install
cp .env.example .env
# Edit .env and add your ANTHROPIC_API_KEY
npm start
# Open http://localhost:3000
```

---

## Environment Variables

| Variable | Required | Description |
|----------|----------|-------------|
| `ANTHROPIC_API_KEY` | ✅ Yes | Your Claude API key |
| `CLAUDE_MODEL` | No | Default: `claude-opus-4-5` |
| `MAX_TOKENS` | No | Default: `2048` |
| `ELEVENLABS_API_KEY` | No | For premium TTS voice |
| `ELEVENLABS_VOICE_ID` | No | Specific ElevenLabs voice |
| `WEATHER_API_KEY` | No | OpenWeatherMap key |
| `NEWS_API_KEY` | No | NewsAPI.org key |

---

## Voice Commands

Say these or type them:

| Command | What happens |
|---------|-------------|
| `Open YouTube` | Opens YouTube in new tab |
| `Open Spotify` | Opens Spotify |
| `Set a timer for 10 minutes` | Sets a browser timer |
| `What time is it?` | Tells current time |
| `Copy hello world` | Copies text to clipboard |
| `Take a screenshot` | Guides for screenshot |
| `Check the weather` | Weather via voice/chat |

---

## Commands

| Command | Description |
|---------|-------------|
| `/search topic` | Research any topic |
| `/code python script` | Generate code |
| `/debug your-code` | Find and fix bugs |
| `/agent objective` | Autonomous multi-step execution |
| `/translate hello` | Translate to 6 languages |
| `/summarize text` | Summarize content |
| `/analyze topic` | Deep analysis |
| `/open app-name` | Launch an application |

---

## Created by Sydney Sider · ALMEER AI v4.0
