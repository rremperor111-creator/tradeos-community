# TradeOS Database Schema

## Users
- id
- email
- username
- password_hash
- created_at

## Trades
- id
- user_id
- symbol
- direction
- entry_price
- exit_price
- stop_loss
- take_profit
- position_size
- risk_percent
- fees
- pnl
- rr
- trade_date
- strategy_id
- notes

## Strategies
- id
- user_id
- name
- description

## Trade Screenshots
- id
- trade_id
- image_path
- type
  - before
  - during
  - after

## Psychology Entries
- id
- trade_id
- confidence
- fear
- focus
- stress
- discipline
- satisfaction
- regret

## Mistakes
- id
- trade_id
- type

## Trade Scores
- id
- trade_id
- entry_quality
- exit_quality
- risk_management
- psychology
- execution
- final_score

## MT5 Accounts
- id
- user_id
- account_number
- broker
- server

## Imported MT5 Trades
- id
- mt5_account_id
- trade_id
