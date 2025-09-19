Trader Behavior Insights – Primetrade.ai Task
Overview

This project was completed as part of the Junior Data Scientist – Trader Behavior Insights assignment.
The objective was to analyze the relationship between Bitcoin Market Sentiment (Fear & Greed Index) and trader performance from Hyperliquid’s historical data, uncovering hidden patterns and generating insights that can support smarter trading strategies.

Datasets

Bitcoin Market Sentiment Dataset

Columns: Date, Classification (Fear/Greed)

Represents overall market sentiment at different points in time.

Historical Trader Data (Hyperliquid)

Columns: account, symbol, execution price, size, side, time, start position, event, closedPnL, leverage, etc.

Captures detailed trade-level information across accounts and instruments.

Approach

Data Loading & Cleaning

Parsed sentiment and historical trading data.

Standardized column names and handled missing values.

Converted time fields into consistent datetime format.

Data Integration

Merged trader data with sentiment dataset using as-of merge (aligning trades to the most recent sentiment state).

Feature Engineering

Classified trades into sentiment states (Fear vs. Greed).

Computed metrics: closed PnL, trade size, win/loss outcomes, leverage usage.

Analysis

Aggregated results by sentiment, account, and symbol.

Calculated:

Number of trades

Total and average PnL

Win rate across conditions

Performed statistical checks (Mann-Whitney test, two-proportion test) where sufficient data existed.

Visualization

Plotted trade performance under Fear vs. Greed.

Visualized distributions of PnL, win rates, and sentiment-based differences.

Account-level and symbol-level leaderboards created.

Key Outputs

Merged dataset with sentiment labels

Aggregated performance metrics by sentiment, account, and symbol

Visualizations highlighting differences in behavior across Fear vs. Greed states

Exported CSVs for downstream use:

merged_trades_with_sentiment.csv

agg_by_sentiment.csv

account_agg.csv

symbol_agg.csv
