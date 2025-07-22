📈 Portfolio Optimization Project

This project applies **Modern Portfolio Theory (MPT)** to construct an optimized equity portfolio using Python. The goal is to identify asset weightings that **maximize risk-adjusted return (Sharpe Ratio)** while maintaining diversification across sectors.

---

##  Methodology

- **Data Collection**: Daily adjusted closing prices for 14 large-cap U.S. stocks across 6 sectors using `yfinance`
- **Preprocessing**: Computed daily log returns and annualized metrics
- **Visualization**: Plotted mean returns, volatility, correlation, and sector breakdowns
- **Risk-Free Rate**: Pulled 10-year Treasury rate via `fredapi`
- **Simulation**: Generated 10,000 random portfolios to create an efficient frontier
- **Optimization**: Used `scipy.optimize` to find portfolio with the **maximum Sharpe Ratio**, under constraints:
  - Individual stock weights between **0% and 25%**
  - Total weights sum to 100%

---

## Key Visuals

-  **Annual Mean Returns** — Highlighting high-growth stocks like NVDA and META  
-  **Volatility Chart** — Exposing risk profiles of each stock  
-  **Efficient Frontier Plot** — Shows optimized portfolio relative to thousands of simulations  
-  **Sector Allocation** — Reveals how the optimizer distributes capital across industries

---

##  Results

AMZN : 0.00e+00
BAC : 5.09e-02
CVX : 0.00e+00
JNJ : 1.99e-01
JPM : 2.50e-01
META : 2.50e-01
NKE : 5.68e-16
NVDA : 2.50e-01
PFE : 6.10e-16
XOM : 0.00e+00

================================================================================
Optimized Metrics
================================================================================
    Returns  Volatility  Sharpe Ratio
0  0.382363    0.220541       1.53515
--------------------------------------------------------------------------------


##  Tools & Libraries

- `Python`, `pandas`, `NumPy`, `matplotlib`, `seaborn`
- `yfinance` – price data  
- `fredapi` – risk-free rate  
- `scipy.optimize` – portfolio optimization

---

## Files

- `Portfolio_Optimization_Mean_Var.ipynb` – full ipynb notebook
- `Portfolio_Optimization_Report.pdf` – detailed write-up with graphs and commentary
