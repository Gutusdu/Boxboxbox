BOX! BOX! BOX! — playable browser prototype
============================================

WHAT'S INCLUDED
- Split-screen game view: pit garage on the left, closed-loop race track on the right.
- Two-player asymmetric setup: mechanic on the iPad, driver controlled by a phone.
- Phone controller with virtual joystick, gas, brake, radio/box and boost.
- Five-digit pairing code using PeerJS WebRTC connection.
- Retro pixel-art-inspired visuals, race timer/laps, tyre wear, damage and pit task progress.
- PWA manifest and service worker for adding the game to the Home Screen.

HOW TO RUN
1. Host the folder on any HTTPS static web host (for example GitHub Pages or Netlify) or a local web server.
2. Open index.html on the iPad, preferably in landscape, and tap “Spiel auf diesem iPad starten”.
3. Open the same hosted URL on the phone and tap “Handy als Controller”.
4. Enter the five-digit code shown on the iPad and tap “Verbinden”.
5. The phone controls the driver; the iPad displays the split-screen and can control the mechanic with WASD / E or touch.

IMPORTANT
- The two devices need internet during pairing; PeerJS's public broker is used for WebRTC signaling. A hosted static URL is required for dependable use across devices. Opening the HTML as a local file on one device will not make it reachable from the other.
- This is a playable prototype, not a finished commercial game. The art is currently drawn procedurally in canvas, not yet a cleaned production tileset/sprite atlas. The circuit and pit tasks are prototype mechanics and can be expanded in the next iteration.
- On iPad, use Safari Share → Add to Home Screen after opening the hosted URL.
