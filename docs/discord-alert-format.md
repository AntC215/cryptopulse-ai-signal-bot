# CryptoPulse Discord Alert Format

This document defines the structure for CryptoPulse Discord trading alerts.

---

## Alert Goals

Each alert should be:

- Clear
- Fast to understand
- Actionable
- Risk-aware
- Easy to review later
- Useful for both beginners and experienced traders

---

## Standard Alert Template

```txt
🚨 CryptoPulse Signal Alert

Asset: ETH
Signal: LONG
Entry: $3,250
Take Profit: $3,360
Stop Loss: $3,180
Confidence: 72%

Reasoning:
EMA trend is bullish, RSI is recovering from oversold conditions, and 1H/4H confirmation supports upside continuation.

Timeframes:
15m: Entry trigger
1h: Bullish confirmation
4h: Trend support

Risk Notes:
Trade is invalidated if price closes below the stop-loss zone or if higher-timeframe trend weakens.
```

---

## Alert Fields

### Asset

The crypto asset being analyzed.

Examples:

- BTC
- ETH
- SOL

### Signal

The signal direction.

Examples:

- LONG
- SHORT
- WATCHLIST
- EXIT

### Entry

The suggested entry price or entry zone.

### Take Profit

The target price or target zone.

### Stop Loss

The invalidation price or risk-control level.

### Confidence

The AI or scoring model confidence level.

### Reasoning

A short explanation of why the trade alert was generated.

### Timeframes

A breakdown of how 15m, 1h, and 4h charts contributed to the signal.

### Risk Notes

Notes explaining invalidation, caution zones, or conditions that weaken the setup.

---

## Premium Alert Concept

Premium Discord alerts may include:

- Chart image
- Entry zone
- Multiple take-profit levels
- Stop-loss zone
- Confidence score
- Setup reasoning
- Market context
- Signal ID
- Timestamp
