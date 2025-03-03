# Trading Strategy Optimization - Nifty50

## Overview

This repository showcases the process of optimizing a trading strategy to outperform the market by developing and testing various techniques. We focused on using the Nifty50 index data from 2020 to 2024 to backtest different strategies. The goal was to develop a robust trading strategy that consistently outperforms the market returns, while maintaining optimal risk-adjusted returns.

The strategies implemented include:
- **Mean Reversion Strategy**
- **EMA Crossover Strategy**
- **Dynamic Stop-Loss using ATR (Average True Range)**

Through the process of optimizing these strategies, we explored the impact of different technical indicators, dynamic stop-loss mechanisms, and capital allocation methods such as the **Kelly Criterion**.

## Objectives

- **Primary Goal:** To develop a trading strategy that outperforms market returns.
- **Risk Management:** Improve risk-adjusted returns by optimizing drawdowns and enhancing the Sharpe ratio.
- **Strategy Optimization:** Experiment with various technical indicators and stop-loss mechanisms to improve overall returns.

## Approach

### 1. **Initial Strategy: Mean Reversion**
   - Implemented a **Mean Reversion Strategy** using Bollinger Bands.
   - Incorporated other technical indicators like **RSI** for more effective decision-making.
   - Introduced the **Kelly Criterion** for optimal position sizing.
   - Applied an **ATR-based Stop-Loss** for dynamic risk management.

### 2. **Improvement Attempts**
   - Tried optimizing the **Bollinger Bands** to make them dynamic.
   - Experimented with using different technical indicators like **RSI** and **EMA** to refine entries and exits.
   - Applied **Kelly Criterion** to determine the optimal amount of capital to allocate for each trade.
   - Despite these adjustments, the strategy did not show significant improvements in returns or risk metrics.

### 3. **Shift to Trend-Based Strategy: EMA Crossover**
   - Moved to a **Trend-Based Strategy** using **Exponential Moving Average (EMA) Crossover**.
   - The strategy was able to outperform the market returns, achieving a better Sharpe ratio and reduced drawdowns.

### 4. **Dynamic Stop-Loss using ATR**
   - Introduced **ATR-based Dynamic Stop-Loss** to adjust the stop-loss level based on market volatility.
   - This addition resulted in improved risk management, minimizing drawdowns and enabling higher returns.

### 5. **Results**
   - The introduction of the **ATR-based dynamic stop-loss** significantly improved the strategy's performance, resulting in higher returns and a more favorable Sharpe ratio.
   - The final strategy had a **Sharpe ratio of 1.49** and a **Maximum Drawdown (MDD) of -12%**, indicating a strong risk-adjusted return.

## Key Metrics

- **Sharpe Ratio**: 1.49
- **Maximum Drawdown (MDD)**: -12%
- **Strategy Type**: Trend-following using EMA crossover with ATR-based dynamic stop-loss.

## Installation

To run this repository and test the strategies, ensure that you have the following libraries installed:

```bash
pip install yfinance pandas numpy matplotlib
