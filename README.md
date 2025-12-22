# That's Not a Hat

An interactive online card game for 2-8 players. A sandbox-style implementation where players interact freely, just like in real life.

## Play Now

**Live Game:** https://thats-not-a-hat-server.kennyphan123.partykit.dev

## About the Game

That's Not a Hat is a memory and bluffing card game. Players draw cards, remember them, and pass them to other players face-down. The challenge is to remember what card you're receiving - or convincingly pretend you do!

### Features

- Real-time multiplayer (2-8 players)
- Drag and drop cards between players
- Flip cards to see/hide them
- Discard pile with history tracking
- Mobile and desktop responsive
- No account required - just share the room code

## How to Play

1. **Create or Join a Game**
   - One player creates a room and shares the 4-letter code
   - Other players join using the code

2. **Draw Cards**
   - Click the deck to draw a card to your hand
   - First card goes to the bottom slot, second to the top

3. **Manage Your Cards**
   - Click your cards to flip them face-up/face-down
   - Drag cards to other players' empty slots
   - Drag cards to the Discard zone to discard (adds a penalty)

4. **Win Condition**
   - A player with 3 penalties loses the game

## Tech Stack

- **Frontend:** Vanilla JavaScript + Vite
- **Backend:** PartyKit (WebSocket server)
- **Hosting:** PartyKit Cloud

## Local Development

### Prerequisites

- Node.js 18+
- npm

### Setup

```bash
# Install dependencies
npm install

# Run development server
npm run dev

# Run PartyKit server locally
npx partykit dev
```

### Deploy

```bash
# Build frontend
npm run build

# Deploy to PartyKit Cloud
npx partykit deploy
```

## Project Structure

```
├── index.html          # Main HTML file
├── src/
│   ├── main.js         # Client-side game logic
│   ├── game.js         # Game state management
│   ├── player.js       # Player rendering
│   ├── card.js         # Card component
│   ├── drag.js         # Drag and drop handling
│   └── styles.css      # Styling
├── party/
│   └── server.js       # PartyKit WebSocket server
├── public/
│   └── cards/          # Card images
└── partykit.json       # PartyKit configuration
```

## License

MIT
