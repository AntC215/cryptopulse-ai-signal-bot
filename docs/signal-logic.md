# CryptoPulse Signal Logic

This document outlines the signal logic concept for the CryptoPulse AI-assisted crypto signal bot.

---

## Supported Assets

The initial bot concept focuses on:

- BTC
- ETH
- SOL

Future versions may support additional crypto assets.

---

## Core Indicators

### EMA

Exponential Moving Averages are used to identify trend direction.

Potential rules:

- EMA20 above EMA50 may indicate bullish momentum.
- EMA20 below EMA50 may indicate bearish momentum.
- EMA crossover may be used as a trigger or confirmation signal.

### RSI

Relative Strength Index is used to identify momentum and overbought / oversold conditions.

Potential rules:

- RSI below 30 may indicate oversold conditions.
- RSI above 70 may indicate overbought conditions.
- RSI recovery from oversold may support a long setup.
- RSI rejection from overbought may support an exit or short setup.

### MACD

MACD may be used as a momentum confirmation tool.

Potential rules:

- Bullish MACD crossover supports long confirmation.
- Bearish MACD crossover supports short confirmation.
- MACD histogram expansion may show trend strength.

### Volume

Volume is used to confirm whether price movement has participation.

Potential rules:

- Rising volume during breakout supports continuation.
- Low volume during breakout may reduce confidence.
- Volume spike with flat price may indicate absorption or hidden accumulation/distribution.

---

## Multi-Timeframe Confirmation

CryptoPulse is designed to compare signals across:

- 15-minute chart
- 1-hour chart
- 4-hour chart

### 15-Minute Timeframe

Used for active entry timing.

### 1-Hour Timeframe

Used for setup confirmation.

### 4-Hour Timeframe

Used for higher-timeframe trend direction.

---

## Signal Types

### Long Signal

A long signal may trigger when:

- EMA trend is bullish
- RSI is recovering from oversold or holding bullish momentum
- Volume confirms move
- 1H and 4H timeframes support upside
- AI confidence score passes the minimum threshold

### Short Signal

A short signal may trigger when:

- EMA trend is bearish
- RSI rejects from overbought or shows weakness
- Volume confirms downside pressure
- 1H and 4H timeframes support downside
- AI confidence score passes the minimum threshold

### Watchlist Signal

A watchlist signal may trigger when:

- Setup is forming but not confirmed
- Confidence score is below publishing threshold
- One or more timeframes are not aligned
- Volume is weak or unclear

---

## Confidence Score Concept

The AI confidence score may consider:

- EMA alignment
- RSI structure
- MACD confirmation
- Volume behavior
- Multi-timeframe alignment
- Trend strength
- Volatility
- Historical setup performance

Example confidence ranges:

| Score | Meaning |
|---|---|
| 80-100 | Strong setup |
| 65-79 | Good setup |
| 55-64 | Watchlist setup |
| Below 55 | Skip / no signal |

---

## Signal Publishing Rule

Signals should only be sent to Discord when:

- Technical setup is valid
- Confidence score is above the required threshold
- Duplicate signal protection passes
- Risk levels are generated
- Alert message is formatted clearly
