# Pinch Catch

A webcam game that runs in the browser. Your hand becomes the controller: pinch your thumb and index finger to grab falling blocks, then let go to throw them into the basket.

Hand tracking uses [MediaPipe Hands](https://github.com/google-ai-edge/mediapipe). No install, no build step, one HTML file.

## How to play

1. Open the page and tap **Start camera**, then allow camera access.
2. Pinch to grab a block. Move your hand to carry it.
3. Open your fingers to throw it into the basket.
4. You have 5 lives. A block that hits the floor costs one.

## Run it

The camera only works over https or on localhost.

- **Vercel or Netlify:** import this repo, no settings needed.
- **GitHub Pages:** Settings > Pages > deploy from the `main` branch, root folder.
- **Local:** open a terminal in this folder and run `python -m http.server 8000`, then visit `http://localhost:8000`.

An internet connection is needed to load the hand-tracking model from a CDN.

## Files

- `index.html`: the whole game (HTML, CSS and JavaScript)

## Ideas for next steps

- 3D scene with depth using Three.js
- Slice mode and finger-gun mode
- Difficulty levels and a saved high score
