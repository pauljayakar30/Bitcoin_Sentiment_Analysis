# Bitcoin Market Sentiment vs. Trader Performance Analysis 📊

## 🎯 Project Objective
The goal of this analysis is to explore the relationship between trader performance and market sentiment. By cross-referencing historical trader execution data with the Bitcoin Fear & Greed Index, this project uncovers hidden behavioral patterns and delivers data-driven insights to drive smarter, more effective trading strategies.

## 📂 Datasets
This analysis integrates two primary data sources:
1.  **Bitcoin Market Sentiment Dataset:** Daily classifications of the market's emotional state (e.g., Fear, Greed, Extreme Greed) via the Fear/Greed Index.
2.  **Historical Trader Data (Hyperliquid):** Granular execution logs including timestamps, execution prices, trade sizes (`Size USD`), and realized profits/losses (`Closed PnL`).

## 🛠️ Tech Stack & Methodology
* **Language:** Python
* **Data Manipulation:** `Pandas` (used for data cleaning, datetime conversion, and grouped aggregations).
* **Data Visualization:** `Plotly Express` (used to generate interactive bar charts for performance trends).
* **Environment:** Google Colab

## 💡 Key Insights & Hidden Patterns
The analysis revealed three critical behaviors that define successful trading performance relative to market mood:

* **The Contrarian Advantage:** There is a clear inverse relationship between public sentiment and trader success. The highest volume of activity (61,837 trades) and the highest total profits (**$3.35 million**) occurred during periods of **"Fear."** This confirms that top-performing traders capitalize on market panic.
* **Strategic Risk Sizing:** Traders dynamically adjust their capital deployment based on sentiment. The average trade size peaked at **~$7,816** during "Fear" markets (maximizing bottom accumulation) and dropped to its lowest point at **~$3,112** during "Extreme Greed" (protecting capital during euphoric peaks).
* **Efficiency in Euphoria:** While overall trade volume decreases during "Extreme Greed," profitability remains high (**$2.7 million**). This suggests that successful traders shift toward a higher-precision, lower-frequency model when the market is overextended.

## 🏁 Conclusion & Strategy
The data definitively supports a **sentiment-driven contrarian approach.** Smarter trading involves:
1.  **Scaling up** position sizes and activity during periods of high market fear to capture maximum upside.
2.  **Reducing exposure** and increasing selectivity during periods of extreme greed to hedge against potential market corrections.

## 🚀 How to Run This Project
1.  Clone this repository to your local machine or GitHub account.
2.  Open the `.ipynb` notebook file in [Google Colab](https://colab.research.google.com/) or Jupyter Notebook.
3.  The notebook is configured to automatically fetch the required datasets using `gdown`.
4.  Run the cells sequentially to reproduce the data merges, statistical tables, and interactive visualizations.

---
**Author:** Vasu Paul Jayakar
