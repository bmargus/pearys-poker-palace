# Peary's Poker Palace
Private play-chip Texas Hold'em for 2–5 seats. No real money.

## Deploy on Render
1. Create a private GitHub repository. Upload the contents of this folder (package.json must be at repository root).
2. In Render create a Web Service connected to that repository. Runtime Node, build command `npm install`, start command `npm start`. Leave root directory blank. Choose an instance plan. Deploy.
3. Open the Render URL, enter your name, and Create private table. Copy invitation and send it to the other players. Each enters their own name and clicks Join invited table. Host can add computer players or remove seats between hands. Deal cards when ready.
4. Voice is off by default; each player can enable it. Browser voices vary.

## Local testing
Run `npm install`, then `npm test`, then `npm start`; visit http://localhost:3000 in separate browser profiles or tabs.

## Limitations
Game and session scores are held in server memory; restart or redeploy clears them. Refresh in the same tab reconnects while the server is running. If someone disconnects mid-hand, they must reconnect to finish the hand. No permanent database or account authentication. Invitation links are private bearer links; do not post publicly. Peary is a photo portrait with spoken commentary, not a fully animated character. Bots use simple randomized strategies. This is a first version; browser multiplayer integration has not been tested in the authoring environment.
