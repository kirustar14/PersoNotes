# MimicNotes 📝

> Notes that think like you — AI that mimics your personal handwriting and note-taking style

## What it does

1. **Upload photos** of your handwritten notes (from your phone camera)
2. **Analyzes** your unique style: bullet vs paragraph, diagram usage, analogies, density, abbreviations, color-coding patterns
3. **Generates** new notes on any topic that look and feel exactly like YOUR notes

## Deploy to GitHub Pages in 2 minutes

```bash
git clone https://github.com/yourusername/mimicnotes
cd mimicnotes
# just push index.html — that's it!
```

Then: **Settings → Pages → main branch / root → Save**

Your app is live at `https://yourusername.github.io/mimicnotes`

## Usage

1. Open the app on your phone
2. Paste your Anthropic API key (stored locally in browser only)
3. Tap the camera zone → photograph your handwritten notes
4. Type a topic
5. Hit **Generate My Notes** ✏️

## API Key

Get a **free** Gemini API key at [aistudio.google.com](https://aistudio.google.com) → Get API Key. No credit card needed. Free tier: 1,500 requests/day. Your key is stored only in your browser's `localStorage` and never sent anywhere except directly to Google's API.

## Tech Stack

- Pure vanilla HTML/CSS/JS — zero build step, zero dependencies
- Calls Claude Vision directly from the browser
- Two-pass AI: first analyzes style profile → then generates style-matched notes
- Deploys as a single `index.html` file

## Style Detection

MimicNotes detects:
- **Note structure**: bullet-heavy, paragraph-heavy, Cornell, outline, mind-map
- **Visual elements**: diagrams, arrows, boxes, highlights, doodles
- **Detail level**: brief keywords → detailed paragraphs
- **Analogy usage**: none / occasional / frequent
- **Writing density**: sparse / moderate / dense
- **Abbreviation patterns**
- **Color coding habits**
- **Personal quirks and flair**
