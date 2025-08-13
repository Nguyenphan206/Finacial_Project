# Monte Carlo Portfolio Optimization

This project implements a **portfolio optimization engine** using **Monte Carlo simulations** to maximize the **Sharpe Ratio** for a set of technology stocks from the NASDAQ.  
It provides **interactive visualizations** of portfolio performance, risk-return profiles, and optimal asset allocations.

---

## Features

- **Data Processing**
  - Reads historical adjusted closing prices for top NASDAQ tech stocks.
  - Calculates daily returns and normalizes prices for fair comparison.

- **Portfolio Construction**
  - Generates random portfolio weight allocations that sum to 100%.
  - Scales initial investments across multiple assets.

- **Performance Metrics**
  - Expected annual return
  - Portfolio volatility (risk)
  - Return on Investment (ROI)
  - **Sharpe Ratio** (risk-adjusted performance)

- **Monte Carlo Simulation**
  - Runs thousands of simulations to explore possible portfolio configurations.
  - Identifies the allocation with the **highest Sharpe Ratio**.

- **Interactive Visualizations**
  - Time-series plots of stock prices, portfolio value, and returns.
  - Scatter plots of risk vs. return with Sharpe Ratio color mapping.
  - Highlighted optimal portfolio point.

---

## Methodology

1. **Load and Clean Data**  
   Import historical stock prices from CSV and calculate daily percentage changes.

2. **Normalize Prices**  
   Scale all stocks so their starting price = 1, enabling proportional investment simulation.

3. **Random Weight Generation**  
   Create random allocations ensuring the sum equals 1.

4. **Portfolio Simulation**
   - Apply weights to scaled prices.
   - Calculate portfolio value, daily returns, and performance metrics.

5. **Monte Carlo Simulation**
   Run thousands of portfolio simulations to explore the return–risk landscape.

6. **Optimization**
   Select the portfolio with the maximum Sharpe Ratio.

---

## Visual Outputs

- **Stock Price Trends**
- **Portfolio Value Over Time**
- **Risk–Return Scatter Plot** (colored by Sharpe Ratio)
- **Optimal Portfolio Marker**
- **Volatility, Return, and Sharpe Ratio Trends**

---

## Tech Stack

- **Python**: `pandas`, `numpy`, `plotly`, `seaborn`, `matplotlib`
- **Jupyter Notebook** / Python Script
- **Monte Carlo Simulation**
- **Financial Metrics Calculation**

---

## Learning Outcomes
- Understanding portfolio theory fundamentals.
- Applying Monte Carlo simulation in finance.
- Calculating and interpreting Sharpe Ratio.
- Building financial dashboards with Plotly and Seaborn.
