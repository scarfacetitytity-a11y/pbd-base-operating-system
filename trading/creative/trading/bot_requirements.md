# trading/bot_requirements.md

## Goal

Build an automated trading research system that can:
- Backtest strategies
- Store results
- Compare indicators
- Track win rate
- Track risk-to-reward
- Track drawdown
- Track best session times
- Track instrument performance
- Help evolve the strategy over time

## Important

The bot should not go live immediately.
First build:
1. Data loader
2. Backtesting engine
3. Strategy rules
4. Results database
5. Trade journal output
6. Dashboard
7. Paper trading mode
8. Risk controls
9. Live execution only after testing

## Suggested Tech Stack

Python:
- pandas
- numpy
- backtesting.py or vectorbt
- ccxt if crypto later
- MetaTrader5 package if using MT5
- FastAPI for backend
- SQLite first, PostgreSQL later
- Streamlit or Next.js dashboard

## Strategy Research Ideas

Test:
- Moving averages
- RSI
- MACD
- VWAP
- Bollinger Bands
- ATR
- Sessions
- Liquidity sweep logic
- Break of structure
- Fair value gaps
- Premium/discount zones
- Multi-timeframe confirmation

## Safety Rules

- No live trading until backtesting and paper trading prove consistency
- Never risk more than defined percentage
- Daily loss limit
- Max trades per day
- Cooldown after loss
- Emergency stop
- No trading during emotional states
