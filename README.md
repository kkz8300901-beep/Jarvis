# Jarvis for Android

An installable voice assistant. It runs in Chrome and sits on your home screen like a normal app.

## What it does
- Listens when you tap Mic, or all the time in Hands-free mode (say "Jarvis, set a timer for 5 minutes").
- Thinks with Claude (needs your own API key).
- Speaks answers aloud, in your phone's voice or a custom ElevenLabs voice.
- Built-in commands: time, date, maths, open YouTube/Gmail/Maps, search, directions, call a number, WhatsApp a number, timer and alarm buttons.

## Step 1: Put the files online (free)
The microphone only works on a secure (https) address, so the files must be hosted. Pick one.

**GitHub Pages**
1. Make a free account at github.com and create a new public repository named `jarvis`.
2. Upload every file in this folder (index.html, manifest.webmanifest, sw.js and the three icon-*.png files).
3. In the repository go to Settings > Pages, set the branch to `main` and the folder to `/ (root)`, and save.
4. After a minute your app is at `https://YOUR-USERNAME.github.io/jarvis/`.

**Netlify Drop**
1. Go to app.netlify.com/drop and drag this folder onto the page.
2. Sign in when asked so the site is kept. You get a link ending in netlify.app.

## Step 2: Install it on your phone
1. Open your link in Chrome on Android.
2. Tap the three dots, then "Add to Home screen" (or "Install app").
3. Open Jarvis from your home screen. Allow the microphone when asked.

## Step 3: Add your keys (Setup button)
- **Claude API key**: create one at console.anthropic.com, add a small amount of credit, and set a monthly spend limit. Paste it into Setup. It is stored only on your phone, never in these files.
- **Claude model**: leave as is. If you get a "model name" error, replace it with a current model name from the Anthropic docs.
- **ElevenLabs key and voice ID** (optional): paste both to use a custom voice. Leave them empty to use your phone's voice. Pick a voice you have the rights to use.

## Good to know
- Hands-free only works while the app is open and the screen is on. Chrome may click or beep each time it restarts the microphone.
- Timer and alarm buttons use Android's Clock app. This depends on your phone and may not work on every device.
- The app cannot read your screen, messages or contacts, or open other apps on its own. Links open when you tap them.
- To update the app later, upload the new files over the old ones. If you still see the old version, close and reopen the app once or twice.
