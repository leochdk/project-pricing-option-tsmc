# Options Pricing & Volatility Smile — TSMC (TSM)

Black-Scholes pricing and implied volatility analysis on TSMC options.

**Data:** Barchart option chain snapshot, close of 22 Sep 2026 (Nov-26 expiry, 59 days) — `chain_tsm.csv`. A live mode (Yahoo Finance) is also available during US market hours.

**Topics covered:**
- Black-Scholes pricing (calls & puts) + put-call parity check
- Implied volatility via a custom Newton-Raphson solver (Brent fallback), computed on bid/ask mid prices
- Market put-call parity check and comparison with Barchart IVs
- Volatility smile analysis: ATM IV vs realized vol, put and call skew

**Key findings:** ATM IV 34% vs 28% realized (earnings on 15 Oct within the option's life), two-sided skew (OTM puts +2 pts, OTM calls +1 pt).

**Stack:** Python · numpy · pandas · scipy · matplotlib · yfinance
