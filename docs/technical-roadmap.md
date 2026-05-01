# CryptoPulse Technical Roadmap

## Phase 1 — Core Signal Logic

- Connect to crypto market data source
- Pull BTC, ETH, and SOL price data
- Calculate RSI
- Calculate EMA20 and EMA50
- Add MACD confirmation concept
- Generate basic long / short signals
- Print signal output locally

---

## Phase 2 — Discord Delivery

- Add Discord webhook integration
- Format signal messages
- Add signal timestamp
- Add asset symbol
- Add entry, take-profit, and stop-loss fields
- Add confidence score field
- Add reasoning text

---

## Phase 3 — Signal Logging

- Log signals to CSV
- Store asset, signal type, timestamp, price, confidence, TP, and SL
- Prevent duplicate alerts
- Track signal history

---

## Phase 4 — Chart Snapshots

- Generate candlestick charts
- Add EMA overlays
- Add RSI visualization
- Add entry marker
- Add take-profit marker
- Add stop-loss marker
- Attach charts to Discord alerts

---

## Phase 5 — AI Confidence Scoring

- Build training dataset from historical signals
- Add model features
- Train RandomForest classifier concept
- Save model with joblib
- Score new signals before publishing
- Only publish signals above confidence threshold

---

## Phase 6 — Performance Analytics

- Track wins and losses
- Calculate average return
- Calculate win rate
- Add daily Discord summary
- Review signal performance by asset
- Review signal performance by timeframe

---

## Phase 7 — Premium Product Layer

- Add premium Discord channel
- Add role-gated alerts
- Add dashboard for users
- Add subscription tier concept
- Add signal archive
- Add market watchlist
