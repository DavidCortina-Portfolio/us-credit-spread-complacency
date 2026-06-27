# US Credit Spread Complacency: A 40-Year Perspective

**Research question:** Is the current level of the US corporate credit spread (1.52% as 
of June 2026) historically low enough to signal complacency in how the market prices 
credit risk — and what does the historical record suggest happens after such episodes?

## Why this matters

A credit spread is the extra yield investors demand to hold corporate bonds over a 
risk-free Treasury — in effect, the market's real-time price for credit risk. When that 
price compresses to historically rare lows, it can mean either that risk has genuinely 
fallen, or that investors are underpricing it.

## Data & Methodology

- **Series:** Moody's Seasoned Baa Corporate Bond Yield relative to the 10-Year Treasury 
  (FRED series `BAA10Y`), daily observations, 1986–2026 (~10,500 days)
- This is a **descriptive and comparative** analysis, not a formal econometric or 
  predictive model — see Limitations

## Key Findings

- The spread has spiked sharply in every recognized credit/economic crisis since 1986, 
  with the 2008 Global Financial Crisis standing alone — at 6.16, nearly double the 
  severity of any other episode, including COVID-19 (4.31)
- As of June 2026, the spread sits at 1.52 — the **6th percentile** of the full 
  historical distribution, among the tightest readings on record
- The naive full-sample correlation between the spread and Treasury yield levels is 
  -0.42, but this is misleading: separated by crisis episode, each period traces its 
  own distinct relationship

## Limitations

This analysis is intentionally descriptive rather than inferential. With ~10,500 daily 
observations exhibiting strong autocorrelation, the effective sample size is far smaller 
than it appears, and any formal hypothesis test would require corrections this project 
does not attempt (e.g., Newey-West standard errors, regime-switching models).

## Repository contents

- `credit_spread_analysis.ipynb` — full analysis notebook (Python, pandas, matplotlib)
- `credit_spread_report.pdf` — one-page summary
- `README.md` — this file

## Tools

Python, pandas, matplotlib, FRED API (Federal Reserve Bank of St. Louis)
