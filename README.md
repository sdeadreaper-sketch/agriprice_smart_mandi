# 🌾 AGRIPrice — Smart Mandi Price Comparison Dashboard

AGRIPrice is a mandi price comparison dashboard designed to help farmers make more informed selling decisions. It lets users compare crop prices across wholesale markets, identify price differences, explore market trends, and set target-price alerts—all in one place.

**Live demo:** https://agriprice7.netlify.app/

![AGRIPrice screenshot](image.png)

> **Note:** This is a  prototype. All prices, trends, AI insights and sync logs are simulated demo data. There is no backend, database or live API connection yet.

---

## Features

- **Price Comparison:** browse mandi price records for 19 crop varieties across 12 markets in 6 states. Filter by category (cereals, vegetables, fruits, pulses, oilseeds, commercial), filter by state, sort by price, name or arrival volume, and switch between card and table views.
- **3-Mandi Arbitrage Analysis:** click any crop to compare its price across three nearby mandis and see the potential extra earnings for a given load.
- **Trends & AI Insights:** a price trend chart drawn on an HTML canvas, plus a market signal panel with a recommended action and target price.
- **Price Alerts:** create and delete alerts that trigger when a crop's price rises above or drops below a target.
- **Farmer Profile:** farm details, notification channel preferences and a mandi watchlist.
- **System Status:** a data provider toggle (demo data vs. an AGMARKNET mode that falls back to demo data) and a mock sync log.
- **Responsive layout** with a separate mobile navigation bar.

## Tech Stack

- HTML5
- [Tailwind CSS](https://tailwindcss.com/) (via CDN)
- Vanilla JavaScript (no frameworks, no build step)
- [Lucide](https://lucide.dev/) icons
- HTML Canvas for the trend chart

## Run Locally

No installation needed.

1. Clone the repo:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   ```
2. Open `index.html` in any modern browser.

An internet connection is required because Tailwind, Lucide and the Inter font load from CDNs.

## Current Limitations

- Data is hardcoded in the page; nothing is fetched from a server.
- Alerts and profile changes live in memory only, so they reset on refresh.
- The AI recommendation and market signal panels show static demo content, not model output.
- Tailwind's CDN build is meant for prototyping, not production.

## Roadmap

- [ ] Integrate real mandi price data from data.gov.in / AGMARKNET
- [ ] Persist alerts and profile settings (backend or `localStorage`)
- [ ] Replace static insights with real price-based calculations
- [ ] Replace the Tailwind CDN with a proper build setup

## Deployment

Hosted on Netlify as a static site.

## Author

ImperioDev
