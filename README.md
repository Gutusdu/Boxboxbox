# BOX BOX BOX — DTM Pit Manager (Prototype 0.1)

A browser-playable, iPad-first pit-team management prototype. The AI drives; players manage the garage, upgrades and pit stops. One host iPad can connect up to three phone controllers (four people total) through PeerJS.

## Features in this prototype
- Responsive iPad/desktop main game and dedicated phone controller (`controller.html`)
- Multiplayer room code, role selection, live state broadcasts and pit-task actions via PeerJS
- DTM Sprint mode with a simple AI race simulation, live timing, fuel/tyre wear and pit stops
- Shared team wallet, reputation, race rewards and purchasable garage upgrades
- Nürburgring 24H special event, gated behind reputation 300 and a €25,000 entry fee
- PWA manifest and SVG icon

## Run locally
Because PeerJS and Google Fonts load from CDNs, an internet connection is needed for those services. You can open `index.html` directly for solo play, but use a local web server for the best experience:

```bash
python3 -m http.server 8000
```

Open `http://localhost:8000` on the iPad/host device. Open `http://<host-lan-ip>:8000/controller.html` on phones on the same Wi-Fi for local hosting of the files. For PeerJS room connections, devices must have internet access and the PeerJS cloud signaling service must be reachable.

## Publish with GitHub Pages
1. Create a GitHub repository.
2. Upload all files from this folder to the repository root.
3. In **Settings → Pages**, select **Deploy from a branch**, choose `main` and `/ (root)`.
4. Open the Pages URL on the iPad. Open `<Pages-URL>/controller.html` on each phone.
5. Create a room on the iPad, then enter the six-digit code on each phone and select a role.

## Multiplayer notes
The static GitHub Pages site is not a multiplayer server. This prototype uses PeerJS's hosted signaling service and WebRTC data connections. It requires internet access and depends on the availability/configuration of that external service. A production build should use a dedicated signaling/backend service, reconnection handling, server-authoritative game state and stronger validation.

## Current prototype limitations
- Race opponents, timing, weather and pit stop durations are simplified simulation systems, not real DTM telemetry.
- The Nürburgring event is a playable event wrapper with simplified lap timing; it does not yet reproduce the full Nordschleife layout or a full 24-hour simulation.
- DTM, Nürburgring and endurance-racing references are used as concepts. This is an unofficial fan prototype and is not affiliated with or endorsed by any championship or circuit. Use original assets/branding if publishing publicly.
- Currency is in-game fictional currency. No real-money payments are implemented.
