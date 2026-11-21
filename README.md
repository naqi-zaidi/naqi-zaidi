# M. Naqi Zaidi

AI Engineering graduate (Ulster University) building quantitative trading tools: risk systems, derivatives pricing and market microstructure.

**Next:** deep-learning mid-price prediction (DeepLOB-style models) on Nasdaq ITCH data rebuilt by my own order book, benchmarked walk-forward against a linear order-flow signal.

### Featured

- **[quant-stack](https://github.com/naqi-zaidi/quant-stack):** a connected market-making research stack, complete through four phases. 333 tests, and every result is reproduced and checked in CI.
  - **C++20 limit order book:** rebuilt Nasdaq's AAPL book from 400,390 LOBSTER messages with zero mismatches. Passed 400,000 property-test calls under ASan/UBSan.
  - **Monte Carlo options pricer:** cuts variance by up to 16,000×. Heston calibrated to 2,874 SPY quotes at a 0.47 vol-point held-out error.
  - **Avellaneda–Stoikov market maker** with a walk-forward order-flow signal: +$249 ± 29/hr out of sample, net of fees, on a simulated market. Replayed on real Nasdaq data, where the edge didn't survive.
  - **Delta hedging and Almgren–Chriss execution:** hedging error matches Derman–Kamal within 3%. A time-of-day impact model predicts realized execution cost within 0.06 bp.
- **[Trading Risk Guardrails](https://github.com/naqi-zaidi/fyp-trading-risk-guardrails):** a Python controller that uses regime and anomaly detection to switch MetaTrader 5 strategies between Allow, Throttle, Pause and Hedge. It was replay-tested on CPI and NFP releases, and ported into quant-stack as a risk overlay that reproduces all 9,000 of its recorded decisions.

**Stack:** Python · C++20 · pybind11 · NumPy / SciPy · GitHub Actions · MQL5 / MetaTrader 5

**Contact:** [LinkedIn](https://www.linkedin.com/in/mohammad-naqi-zaidi-302682326/) · [zaidinaqi52@gmail.com](mailto:zaidinaqi52@gmail.com)
