# Market Exploration Workspace

## Status

This is a small exploratory workspace containing two different ideas:

1. `Oil Venezula.ipynb` downloads adjusted prices for CVX, XOM, and COP over a short date window and inspects their correlation.
2. `data/` contains small Polymarket and Kalshi exports related to a Venezuela leadership market.

These materials do not yet form one reproducible event study, and the repository should not be presented as a completed stock-by-industry analysis.

## Reproduce the notebook

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
jupyter notebook "Oil Venezula.ipynb"
```

The notebook downloads current historical data through `yfinance`; upstream revisions and the selected date window can affect results.

## Interpretation limits

- Correlation over one short window does not establish a stable relationship or causal exposure.
- The notebook does not currently connect equity returns to the prediction-market exports.
- A complete event study would define an event timestamp, return baseline, estimation window, abnormal-return method, and robustness checks.

The audit recommends either splitting these ideas or renaming the repository to match a completed analysis. That account-level action requires explicit approval.
