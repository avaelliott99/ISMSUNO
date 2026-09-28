# ISMSUNO Music Studio

A single-page AI music generator built on the [Suno API](https://docs.sunoapi.org). It's a plain static site with no build step and no server code.

## Features
- **Bring your own API key**: users paste their [sunoapi.org](https://sunoapi.org/api-key) key in the app. It's stored only in their browser and sent only to `api.sunoapi.org`.
- **Live credit balance** in the header.
- **Simple mode**: describe a song and Suno writes the lyrics and music.
- **Custom mode**: title, style, your own lyrics (or ✨ AI-written lyrics), vocal gender, duration, excluded styles, and advanced sliders (style weight, weirdness, audio weight, variety).
- **Models**: V6, V6 Mini, V6 Wild.
- **Library**: stream previews while tracks finish, then play, download MP3, convert to WAV, extend a track, view or reuse its lyrics, and search. The library is saved in local storage, and in-progress jobs resume after a page reload.

## Deploy to Netlify
1. Connect this repo in Netlify (or drag-and-drop the `public/` folder).
2. Settings come from `netlify.toml`: publish directory `public`, no build command.
3. Open the site, click **API key**, and paste your key.

## Run locally
Serve the `public/` folder with any static server, e.g. `npx serve public`.

> Suno keeps generated audio for about 14 days, so download anything you want to keep.
