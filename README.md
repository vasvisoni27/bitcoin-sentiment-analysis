# bitcoin-sentiment-analysis
# Bitcoin Market Sentiment vs Trader Performance Analysis
## Objective

This project analyzes the relationship between Bitcoin market sentiment and trader performance using historical trading data from Hyperliquid and the Bitcoin Fear & Greed Index.
The goal is to identify how different market sentiment regimes affect profitability, win rates, trading activity, and trading strategies.
---

## Datasets

### 1. Bitcoin Fear & Greed Index
Columns:
* date
* classification
* value
Sentiment categories:
* Extreme Fear
* Fear
* Neutral
* Greed
* Extreme Greed

### 2. Hyperliquid Historical Trader Data

Key columns:
* Account
* Coin
* Execution Price
* Size USD
* Direction
* Closed PnL
* Fee
* Timestamp IST

### Dataset Source
The datasets used in this project were provided as part of the assignment. The original dataset links are included in the assignment instructions and can be accessed from the provided source URLs.
---

## Methodology
1. Loaded and inspected both datasets.
2. Checked for missing values and data quality issues.
3. Standardized date formats.
4. Merged trader data with sentiment data using trading dates.
5. Analyzed profitability by sentiment category.
6. Calculated win rates across sentiment regimes.
7. Compared Long and Short trade performance.
8. Evaluated trading activity under different market conditions.
9. Generated visualizations and summary statistics.
---

## Key Findings

### 1. Profitability by Sentiment

| Sentiment     | Total PnL | Average PnL |
| ------------- | --------: | ----------: |
| Fear          | 3,357,155 |       54.29 |
| Extreme Greed | 2,715,171 |       67.89 |
| Greed         | 2,150,129 |       42.74 |
| Neutral       | 1,292,921 |       34.31 |
| Extreme Fear  |   739,110 |       34.54 |

**Observation:** Fear generated the highest total profit, while Extreme Greed produced the highest average profit per trade.
---

### 2. Win Rate Analysis

| Sentiment     | Win Rate (%) |
| ------------- | -----------: |
| Extreme Greed |        46.49 |
| Fear          |        42.08 |
| Neutral       |        39.70 |
| Greed         |        38.48 |
| Extreme Fear  |        37.06 |

**Observation:** Extreme Greed achieved the highest win rate, while Extreme Fear showed the lowest.
---

### 3. Long vs Short Strategy Performance

* Long positions outperformed during Greed and Extreme Greed periods.
* Short positions outperformed during Fear and Extreme Fear periods.
This suggests that market sentiment can be used as a signal for directional bias.
---

### 4. Trading Activity

| Sentiment     | Percentage of Trades |
| ------------- | -------------------: |
| Fear          |               29.28% |
| Greed         |               23.82% |
| Extreme Greed |               18.93% |
| Neutral       |               17.84% |
| Extreme Fear  |               10.13% |

**Observation:** Fear periods accounted for the largest share of trading activity.
---

## Visualizations

The project includes the following charts:

* Total Profit by Market Sentiment
* Win Rate by Market Sentiment
* Long vs Short Performance by Sentiment

These charts are available in the `charts/` directory.
---
## Conclusion

The analysis demonstrates a clear relationship between Bitcoin market sentiment and trader performance.
Key conclusions:

* Fear periods generated the highest overall profits due to increased trading activity.
* Extreme Greed produced the highest average profit per trade and the highest win rate.
* Long strategies performed best during Greed conditions.
* Short strategies performed best during Fear conditions.

These findings suggest that incorporating sentiment indicators into trading strategies may improve profitability and risk management.
---

## Technologies Used
* Python
* Pandas
* Matplotlib
* Jupyter Notebook


