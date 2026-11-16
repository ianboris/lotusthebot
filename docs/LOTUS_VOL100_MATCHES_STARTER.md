# Lotus Volatility 100 (1s) Matches starter

Import file: `lotus_vol100_matches_1tick.xml`

## Configuration
- Market: Derived Indices / Continuous Indices / Volatility 100 (1s), symbol `1HZ100V`
- Contract: Digits / Matches (`DIGITMATCH`)
- Prediction barrier: 5 (editable in the Trade options block)
- Duration: 1 tick
- Stake: 1 AUD (verify the account currency and minimum stake before any live use)
- Candle interval: 1 minute (metadata/default interval; Matches settles on ticks)
- Restart buy/sell on error: off
- Restart last trade on error: off
- Martingale/recovery staking: none
- Session stop: stops when cumulative session PnL is at or below -1 AUD or at or above +2 AUD
- No Sell block; contracts settle at expiry

## Important limitations
This is an importable execution/risk-control starter, **not a proven profitable strategy**. It uses a fixed prediction digit (5); it does not estimate a predictive edge. A fair 0-9 last digit has a 10% unconditional match probability before payout economics. The session guard limits continuation but cannot create an edge or prevent a single contract from losing its full stake.

The XML does not choose the Deriv account. The account selected in the Deriv login/session controls whether quotes and purchases are demo or live. Import it, inspect the market/contract/stake/prediction, and do not press Start on a live account until the strategy has passed demo and out-of-sample testing.

No live trade was started by preparing this file.
