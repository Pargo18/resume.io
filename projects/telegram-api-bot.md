---
layout: single
title: "Trading bot with Telegram API integration for automated alerts"
permalink: /projects/telegram-api-bot/
---

# Smart Crypto Rebalancing Bot

<p align="center">
  <img src="/logos/telegram.png" alt="" />
</p>

A lightweight Python-based bot that monitors a mock cryptocurrency portfolio using live CoinGecko prices and alerts you via Telegram if it deviates from a defined allocation.

This repo attempts to vreate a portfolio balancing bot together with a Telegram API integration for automated pre-scheduled real-time alerts

## Features
- Simulates crypto holdings (BTC, ETH)
- Uses live market prices from the CoinGecko API
- Compares current vs. target allocation (e.g., 60% BTC / 40% ETH)
- Sends alerts via Telegram when rebalancing is needed
- Easy to customize and extend

## Tech Stack
- Python 3
- Requests (API interaction)
- Telegram Bot API
- `schedule` (for periodic checks)

## How It Works
1. Define your target allocation and mock portfolio
2. Fetch live prices from CoinGecko
3. Calculate current portfolio distribution
4. Compare to the target allocation
5. If deviation exceeds threshold, alert via Telegram

## Example Alert
```
Rebalancing Alert:

SELL BTC | Current: 65.21%, Target: 60.00%
BUY ETH  | Current: 34.79%, Target: 40.00%
```

## Next Steps
- Connect to live exchange portfolio via Binance API
- Enable actual trade execution


For the full code, visit the [GitHub repository](https://github.com/Logikon-Solutions/Trading-bot-with-Telegram-API-integration-for-automated-alerts)
