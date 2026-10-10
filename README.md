# Frank’s Trader v10.3 — Checked Multi-Source Intelligence

# Frank's Trader v10 — Multi-Source Intelligence

v10 adds SEC EDGAR as an independent fundamental-data fallback/cross-check to FMP.

- Nasdaq Trader remains discovery universe.
- FMP remains market/quote and first-pass fundamentals.
- SEC EDGAR companyfacts supplies XBRL revenue, income, cash flow, balance-sheet evidence when available.
- SEC submissions add recent filing awareness.
- Missing factors remain unscored; 0% coverage now means 0 confidence.
- New positions: BUY / WATCH / AVOID / RESEARCH.
- Owned positions: HOLD / TRIM / SELL / RESEARCH.
- Paper only. No brokerage execution.

SEC automated access is deliberately low-volume and server-side. No additional API key is required.


## v10.3 verification pass
- Rechecked SEC foreign-private-issuer handling against current SEC XBRL guidance.
- Supports US-GAAP and IFRS facts; 20-F/40-F annual facts and 6-K point-in-time facts.
- Missing evidence remains unscored; 0% coverage = 0 confidence.
- SEC failure messages are surfaced for diagnosis rather than replaced with neutral scores.
- Paper-only decision logic retained.
- Package syntax and ZIP integrity checked before release.
