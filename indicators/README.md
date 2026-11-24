# CNTRLR FX - Price Action Setups

A TradingView Pine Script v6 indicator (`cntrlr_fx_setups.pine`) that automates the
price-action framework: **Breakout**, **Fakeout**, **Onion Play**, **Continuation**,
and **Reversal** setups, each drawn with a stop-order entry line, a stoploss line,
and a label. Tight signal candles are auto-tagged `Celery Play`.

## Install

1. Open TradingView -> Pine Editor -> New blank indicator.
2. Paste the contents of `cntrlr_fx_setups.pine`.
3. Click "Add to Chart".

## Tuning

- **Pivot Lookback** - how many bars on each side confirm a swing high/low.
- **Zone Tolerance (x ATR)** - how close a new pivot must be to an existing
  level to count as a retest instead of a new level.
- **Onion Min Bars** - how long a range must hold before the pending stop
  orders tighten into "Onion Play" mode.
- Setup categories and colors can be toggled per-type in the indicator's inputs.

See the comment header in the script for the assumptions made when translating
the discretionary rules (e.g. "Celery Play", the BOPCH/BOPCL trend
continuation/reversal logic) into automated conditions.
