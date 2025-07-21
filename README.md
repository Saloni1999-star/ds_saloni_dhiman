#  Web3 Trading Assignment – Sentiment vs Trader Behavior

**Candidate Name:** Saloni Dhiman  
**Submission Date:** July 2025

---

##  Objective

To analyze how trader behavior—**profitability**, **risk-taking**, **volume**, and **trade direction**—aligns or diverges from overall **Bitcoin market sentiment** using two datasets:

1. **Bitcoin Fear & Greed Index**
2. **Historical Trader Data from Hyperliquid**

---

##  Project Structure

ds_saloni_dhiman/
├── notebook_1.ipynb # Sentiment vs behavior analysis
├── notebook_2.ipynb # Deep dive: PnL vs Trade Size
├── csv_files/
│ ├── trader_data.csv # Raw trader activity
│ ├── sentiment_data.csv # Bitcoin sentiment (daily)
│ └── merged_data.csv # Cleaned & merged dataset
├── outputs/
│ ├── avg_pnl_by_sentiment.png
│ ├── avg_trade_size_by_sentiment.png
│ ├── trade_direction_by_sentiment.png
│ ├── pnl_vs_size_heatmap.png
│ └── pnl_vs_size_scatter.png
├── ds_report.pdf # Final PDF summary
└── README.md # You’re here!


---

##  Key Insights

###  Avg Closed PnL by Sentiment
| Sentiment       | Avg PnL (USD) |
|-----------------|---------------|
|   Extreme Greed | **67.89**     |
|   Fear          | 54.29         |
|   Greed         | 42.74         |
|   Extreme Fear  | 34.53         |
|   Neutral       | 34.30         |

-  Traders are **most profitable during Extreme Greed** with **Avg PnL = $67.89**
- 🔻 Profitability drops by **49.5%** in Neutral conditions compared to Extreme Greed

---

###  Avg Trade Size by Sentiment

| Sentiment       | Avg Trade Size (USD) |
|-----------------|----------------------|
|   Fear          | **7816.11**          |
|   Greed         | 5736.88              |
|   Extreme Fear  | 5349.73              |
|   Neutral       | 4782.73              |
|   Extreme Greed | 3112.25              |

-  Trade sizes are **highest during Fear**, suggesting **riskier trades** or **desperation during downturns**
-  **Extreme Greed** leads to **lowest trade sizes**, possibly due to overconfidence or safe profit booking

---

###  Trade Direction vs Sentiment

-  **Long Trades** dominate during **Greed** (65% of trades were long)
-  **Short Trades** peak during **Extreme Fear** (up to 58% of trades)
-  During **Neutral** sentiment, trade direction is almost balanced (long ≈ short)

---

###  Additional Insights

-  Outlier traders with unusually large PnLs (e.g., > $3000) were removed to stabilize trend lines
-  Traders with mid-sized trades ($4k–$8k) showed the **most stable profit range**
-  In Extreme Greed, **PnL variance is highest**—risky bets with both high gains and losses

---

##  Additional Observations (Data-Driven)

-  **Standard deviation of PnL** is highest in **Extreme Greed** (`std_dev = 510.22`)
-  **Volume traded per trader** was 27.4% higher in Fear than Greed
-  In **Extreme Fear**, 1 in 5 traders had a negative PnL exceeding -$100
-  **Correlation (r)** between trade size and PnL is very low: `r ≈ 0.07` → almost no linear relationship
-  Median PnL across all sentiments: **$41.22** (vs mean: **$46.15** → suggests skew due to high earners)

---

## Conclusion

-  **Greedy sentiment correlates with higher profits**, but more volatility and lower trade sizes.
-  **Fearful traders take larger trades**, possibly indicating loss-recovery attempts or panic trades.
-  **Trade direction flips with sentiment**, confirming psychological impact on market positions.
-  **Trade size ≠ profit** — high-risk trades don’t guarantee better outcomes.
-  **Traders are most profitable when optimistic**, but most active when fearful.
-  **Outlier removal is critical** for reliable analysis and trend clarity.
-  The **Fear & Greed Index** is a strong behavioral proxy in Web3 trading analytics.

---

## Deliverables

- `notebook_1.ipynb` – Main sentiment vs behavior analysis  
- `notebook_2.ipynb` – Focused study on trade size vs profit  
- Datasets in `csv_files/`  
- Visual outputs in `outputs/`  
- Summary report `ds_report.pdf`  
- This README.md

---

## Tools Used

- **Python**: pandas, seaborn, matplotlib  
- **Platform**: Jupyter Notebooks / Google Colab  
- **Version Control**: Git & GitHub

---

##  Contact

- GitHub: [@saloni260](https://github.com/saloni260)  


