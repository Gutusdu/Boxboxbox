BOX! BOX! BOX! — 2-player mobile/iPad prototype
================================================

INCLUDED
- Split-screen prototype: pit garage + closed-loop circuit.
- iPad host role and phone driver controller.
- Five-digit room code with PeerJS WebRTC signaling.
- Phone controls: steering stick, gas, brake, radio/box, boost.
- iPad mechanic controls: WASD + E or touch.
- Lap timer, lap count, tyre wear, damage and pit-task progress.
- PWA manifest/service worker for Add to Home Screen.
- Concept artwork included locally in assets/:
  * racetrack-concept.png — closed-loop track/paddock visual reference.
  * character-car-concept.png — car/driver/mechanic visual reference.

PUBLISH ON GITHUB PAGES
1. Unzip the package.
2. Upload the CONTENTS of the BOX_BOX_BOX folder to the root of your GitHub repository.
   index.html must be at the repository root, with manifest.json, sw.js and assets/ beside it.
3. In Settings > Pages, choose Deploy from a branch, branch main, folder /(root).
4. Open the published HTTPS URL on the iPad and choose “SPIEL AUF DIESEM iPad STARTEN”.
5. Open the same URL on the phone, choose “HANDY ALS CONTROLLER”, enter the code shown on the iPad and press VERBINDEN.

CONNECTION NOTES
- Both devices need internet during initial pairing. PeerJS uses its public signaling service; actual WebRTC connectivity can still be blocked by some networks. GitHub Pages hosts static files only; it is not a multiplayer server.
- Keep the iPad host page open while connecting the phone. If the code fails, reload both devices and create a fresh code.
- This package has not been live-tested on the user's devices.

IMPORTANT SCOPE / ART STATUS
This is a prototype, not a finished production game. The active game scene still draws its simple pixel-style car, track and mechanic procedurally in Canvas. The supplied concept images are bundled and shown in the start menu as visual references; they are not yet cleaned individual animation frames or a fully tiled playable track. The earlier exact animation sprite sheets were not present in the available project files, so they have not been falsely represented as integrated. The pit stop and lap systems are basic prototype mechanics and need further testing/polish.

On iPhone/iPad Safari, use Share > Add to Home Screen to install the PWA shortcut.
