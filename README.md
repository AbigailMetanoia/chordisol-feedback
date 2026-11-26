# Chordisol Feedback

A feedback wall for the Chordisol app. Visitors write a short note, it sticks to the wall with a burst of stars and music notes, then a "Thank You So Much!" screen shows the App Store QR code.

## Run it

Open `index.html` through any static server, for example:

```sh
npx serve .
```

(Opening the file directly with `file://` blocks the Lottie animation from loading.)

## Where feedback is stored

- **On claude.ai (the artifact version):** notes are saved in the artifact's shared database and appear live for everyone who opens it.
- **Hosted anywhere else (GitHub Pages, local server):** notes are saved in that browser's `localStorage`, so they stay on that one device. This works for an exhibition booth on one laptop. To collect notes from many devices, connect a backend such as Firebase or Supabase.

## Sound

All sound effects are synthesized with the Web Audio API (no audio files). The speaker button in the top-right corner mutes them.
