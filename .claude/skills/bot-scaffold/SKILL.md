---
name: bot-scaffold
description: Scaffold or extend the Python trading bot / backtesting project defined in bot_requirements.md — data loader, backtesting engine, strategy rules, results database, trade journal output, dashboard, paper trading, risk controls. Use when the user asks to start building the trading bot, add a module to it, or set up the project skeleton.
---

# Bot Scaffold

Reference: `trading/creative/trading/bot_requirements.md`.

## Build order — do not skip ahead

1. Data loader
2. Backtesting engine
3. Strategy rules
4. Results database
5. Trade journal output
6. Dashboard
7. Paper trading mode
8. Risk controls
9. Live execution — only after everything above is proven out

If the user asks to jump straight to live execution or skip paper trading, push back. That's the one hard rule in bot_requirements.md.

## Tech stack

- Python: pandas, numpy
- Backtesting: `backtesting.py` or `vectorbt`
- `ccxt` if/when crypto is added
- `MetaTrader5` package if using MT5
- Backend: FastAPI
- Storage: SQLite first, PostgreSQL later
- Dashboard: Streamlit or Next.js

## Strategy building blocks to support

Moving averages, RSI, MACD, VWAP, Bollinger Bands, ATR, session filters, liquidity sweep logic, break of structure, fair value gaps, premium/discount zones, multi-timeframe confirmation — these map to the Sniper v1.0 model in `trading/trading_framework.md`, so strategy rules should be expressible in those terms.

## Safety rules to hard-code, not just document

- No live trading until backtesting + paper trading prove consistency
- Max risk per trade as a config value, never hardcoded inline
- Daily loss limit
- Max trades per day
- Cooldown after a loss
- Emergency stop switch

## When scaffolding

- Create a clean folder structure (e.g. `bot/data/`, `bot/backtest/`, `bot/strategies/`, `bot/db/`, `bot/journal/`, `bot/dashboard/`, `bot/risk/`)
- Keep the first version simple — working beats flashy. Follow `app_build/app_vision.md`: backend organisation before UI polish.
- Never commit API keys, broker logins, or secrets — use `.env` and make sure it's gitignored.
