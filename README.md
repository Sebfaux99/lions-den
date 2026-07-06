# 🦁 Lions Den
### Private Betting Intelligence Dashboard

---

## Run locally (30 seconds)

**Option A — Open directly in your browser (no install needed)**
Just double-click `index.html` — it works as a standalone file.

**Option B — Run as a proper web app**
```bash
npm install
npm start
```
Then open → http://localhost:3000

---

## Pages

| Page | What it does |
|---|---|
| **Dashboard** | KPI cards, P&L chart, sport allocation, recent activity |
| **Bet Log** | Log bets, mark won/lost, filter, delete |
| **Holdings** | Sport-by-sport breakdown — ROI, win rate, staked |
| **Analytics** | P&L by sport, bookmaker breakdown, best/worst markets |
| **Insights** | Auto-generated signals from your real data + market alerts |
| **Markets** | Best odds comparison across bookmakers |
| **Concierge** | VIP and white-glove service options |
| **Settings** | Name, bankroll, export CSV, clear data |

---

## Key features

- **Zero fake data** — every number on the dashboard comes from your logged bets
- **Log a bet** — sport, event, market, bookmaker, stake, odds, CLV, notes
- **Instant settlement** — WON / LOST buttons on every open position
- **Auto insights** — generates signals based on your real performance
- **Export CSV** — download all your bets as a spreadsheet any time
- **Persists across sessions** — everything saves in your browser's localStorage

---

## Deploy free (Netlify — easiest)

1. Go to netlify.com and sign up free
2. Drag and drop the `lions-den` folder onto the Netlify dashboard
3. Done — you'll get a live URL in 30 seconds

## Deploy free (Vercel)

1. Push this folder to a GitHub repo
2. Go to vercel.com → Import project → pick your repo
3. Deploy — live in under a minute

## Deploy on Replit (no credits needed)

1. Create a new Node.js Repl
2. Upload the three files: `index.html`, `server.js`, `package.json`
3. Click Run

---

## Upgrade path — live odds

When ready to connect real odds data:
1. Sign up at https://the-odds-api.com
2. Create `routes/markets.js` in a backend folder
3. Call `GET https://api.the-odds-api.com/v4/sports/{sport}/odds?apiKey=YOUR_KEY`
4. Replace the `STATIC_MARKETS` array in `index.html` with a fetch to your new route

The frontend is already structured to swap this in without touching any other code.
