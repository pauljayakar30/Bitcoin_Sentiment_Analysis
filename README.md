# Bitcoin Market Sentiment vs. Trader Performance Analysis 📊

## Project Overview
This project explores the relationship between trader performance and general market sentiment in the cryptocurrency space. By cross-referencing historical trader execution data with the Bitcoin Fear & Greed Index, the objective is to uncover hidden behavioral patterns and deliver data-driven insights to optimize trading strategies.

## Datasets Used
1. **Bitcoin Market Sentiment Dataset:** Contains daily classifications of the market's emotional state (e.g., Fear, Greed, Extreme Greed).
2. **Historical Trader Data (Hyperliquid):** Contains granular execution data including transaction timestamps, execution prices, bet sizes (`Size USD`), and realized profits/losses (`Closed PnL`).

## Tech Stack
* **Language:** Python
* **Data Manipulation:** Pandas (Data merging, datetime conversion, grouped aggregations)
* **Data Visualization:** Plotly Express (Interactive bar charts)
* **Environment:** Google Colab

## Key Insights & Hidden Patterns
Through data cleaning and aggregation, several key patterns emerged regarding how market sentiment dictates trader behavior and profitability:

* **The Contrarian Strategy is Optimal:** The data reveals an inverse relationship between public sentiment and trader success. The highest volume of trading activity and the highest aggregate profits ($3.35 million) were realized when the market sentiment was classified as "Fear."
* **Extreme Greed Requires High Efficiency:** During periods of "Extreme Greed," traders executed significantly fewer trades. However, they maintained a high level of profitability ($2.7 million). This suggests a shift toward highly selective, high-probability setups rather than volume trading.
* **Dynamic Risk Sizing:** Traders dynamically adjust their deployed capital based on sentiment. The average capital deployed per trade peaked at ~$7,816 during "Fear" markets (maximizing bottom accumulation) and dropped to its lowest at ~$3,112 during "Extreme Greed" markets (protecting capital during euphoric peaks).

## Conclusion
The analysis definitively supports a contrarian, risk-managed trading approach. The most profitable behavior involves deploying heavier capital during market fear and aggressively scaling down position sizes during extreme greed.

## How to Run This Project
1. Clone this repository.
2. Open the `.ipynb` notebook file in [Google Colab](https://colab.research.google.com/) or Jupyter Notebook.
3. The notebook is configured to automatically pull the necessary datasets via `gdown`. Simply run the cells sequentially to reproduce the data merges and Plotly visualizations.

---
**Author:** Vasu Paul Jayakar
