
# MEMESCOPE — Solana Memecoin Tracker

A dark-mode trading terminal for discovering and monitoring
Solana memecoin markets using public DEX Screener data.

## Features

- Solana trading pair discovery
- Token name, symbol and address search
- USD price and 24-hour price change
- Liquidity, volume and market cap / FDV
- Gainers and losers filters
- Browser-based watchlist
- Top movers dashboard
- Mini price charts based on observed samples
- Automatic refresh every 60 seconds
- Responsive terminal-style UI
- Direct links to DEX Screener token pages

## Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript
- DEX Screener API
- Browser localStorage

No framework, build step, API key, or backend is required
for this basic public-data demo.

## Getting Started

### Option 1: Run locally

1. Clone the repository:

   git clone https://github.com/YOUR_USERNAME/memecoin-tracker.git

2. Open the project folder.
3. Open `index.html` in a modern browser.

If direct file access causes problems, use a local static
server or VS Code Live Server.

### Option 2: Deploy with GitHub Pages

1. Push all project files to the `main` branch.
2. Open your repository on GitHub.
3. Go to Settings → Pages.
4. Under Build and deployment, select:
   - Source: Deploy from a branch
   - Branch: main
   - Folder: / (root)
5. Click Save.
6. Wait for GitHub Pages to publish the website.

Your site will usually be available at:

https://YOUR_USERNAME.github.io/memecoin-tracker/

Replace `YOUR_USERNAME` with your GitHub username.

## API

This project uses the public DEX Screener API.

Token and pair search:

https://api.dexscreener.com/latest/dex/search?q=bonk

The app searches several discovery queries and filters
the returned pairs to the Solana network.

Official API reference:

https://docs.dexscreener.com/api/reference

## Data Limitations

- Discovery queries do not cover every Solana token.
- Trending results are based on the tokens discovered
  by the app, not a universal market ranking.
- Data availability and refresh frequency depend on
  the upstream API and network connectivity.
- The mini chart records observed prices while the page
  is running. It is not a historical market chart.
- Market cap may fall back to FDV when market cap is
  unavailable. Treat this value as an estimate.
- A token's presence does not imply safety or legitimacy.

## Security

- No wallet connection is required.
- No seed phrase or private key is requested.
- Watchlist data is stored in local browser storage.
- External trading links open in a new tab.

## Disclaimer

This project is for educational and informational
purposes only. It is not financial advice.

Memecoins can be extremely volatile, illiquid, or scams.
Verify token mint addresses, liquidity, ownership and
other risks independently before trading.

## License

MIT
