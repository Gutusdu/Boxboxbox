BOX! BOX! BOX! — 2-Player Browser Prototype
==========================================

HOSTING
- Upload the CONTENTS of this folder to the root of your GitHub Pages repository.
- Keep index.html, manifest.json, sw.js, and assets/ together.
- Open the published HTTPS address on the iPad and choose “SPIEL AUF DIESEM iPad STARTEN”.
- Open the same address on the phone, choose “HANDY ALS CONTROLLER”, enter the five-digit code and connect.
- Keep internet enabled on both devices during pairing. PeerJS public signaling is used.

CURRENT FEATURES
- Existing split-screen layout is preserved: pit garage on the left, closed loop track on the right.
- Two-device PeerJS pairing and phone driver controls (joystick, gas, brake, radio/box, boost).
- The race car advances continuously around a closed oval track instead of jumping according to elapsed time.
- Steering influences speed; tyre wear, damage, lap counter and boost remain active.
- Mechanic can be moved around the garage with WASD and by tapping a destination on the garage canvas; holding/interacting progresses pit work.
- PWA files for adding the site to the iPhone/iPad Home Screen.

ART
- assets/racetrack-concept.png and assets/character-car-concept.png are the supplied concept sheets for visual reference.
- The in-game canvas still draws prototype pixel graphics procedurally. The concept sheets are not yet cleaned, individual animation sprite atlases; those need the original separate animation frames to be integrated correctly.

NOTE
This is an improved playable prototype, not a finished commercial game. Test the two-device connection and gameplay on the actual devices after publishing. If PeerJS reports an error, note the exact error shown on the screen.
