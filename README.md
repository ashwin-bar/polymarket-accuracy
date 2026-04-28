# Polymarket Calibration Engine

This project analyzes the forecasting accuracy of Polymarket using on‑chain data from Dune Analytics via the `dune-client` Python SDK.[1]

The notebook:

- Pulls ~100k+ resolved Polymarket markets from Dune
- Computes Brier Score decay from 30 days before resolution to 1 day before
- Breaks Brier scores down by category (Politics, Crypto, Sports, Finance/Macro, Esports/Gaming, Other)
- Builds a calibration curve 7 days before resolution to test whether implied probabilities match actual outcomes

## How to run

1. Open the notebook: `polymarket_calibration_engine.ipynb`
2. Replace `YOUR_DUNE_API_KEY_HERE` in the first code cell with your own Dune API key (from dune.com/settings/api)
3. Run all cells

The static version on GitHub already shows all charts and commentary; running the notebook just refreshes the data.
