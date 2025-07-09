# Web3 Trading Assignment – Sentiment vs Trader Behavior 📊

**Candidate Name:** Saloni Dhiman  
**Submission Date:** July 2025  

---

## Objective

To analyze how trader behavior—profitability, risk-taking, volume, and direction—aligns or diverges from overall **Bitcoin market sentiment** using two datasets:

1. **Bitcoin Fear & Greed Index**
2. **Historical Trader Data from Hyperliquid**

---

##  Project Structure

ds_saloni_dhiman/
├── notebook_1.ipynb # Main analysis notebook
├── notebook_2.ipynb # Deep dive on trade size vs PnL
├── csv_files/
│ ├── trader_data.csv # Raw trader data
│ ├── sentiment_data.csv # Market sentiment data
│ └── merged_data.csv # Cleaned & merged dataset
├── outputs/
│ ├── avg_pnl_by_sentiment.png
│ ├── avg_trade_size_by_sentiment.png
│ ├── trade_direction_by_sentiment.png
│ ├── pnl_vs_size_heatmap.png
│ └── pnl_vs_size_scatter.png
├── ds_report.pdf # Final PDF report
└── README.md # Project summary


---

##  Key Insights

###  Average Closed PnL by Sentiment:

| Sentiment       | Avg PnL (USD) |
|-----------------|---------------|
| Extreme Greed   | 67.89         |
| Fear            | 54.29         |
| Greed           | 42.74         |
| Extreme Fear    | 34.53         |
| Neutral         | 34.30         |

---

###  Average Trade Size (USD):

| Sentiment       | Avg Trade Size (USD) |
|-----------------|----------------------|
| Fear            | 7816.11              |
| Greed           | 5736.88              |
| Extreme Fear    | 5349.73              |
| Neutral         | 4782.73              |
| Extreme Greed   | 3112.25              |

---

###  Trade Direction vs Sentiment:

- More **Long trades** during **Greed**
- More **Short trades** during **Extreme Fear**

---

###  Additional Analysis:

- Hexbin and scatter plots show weak correlation between **trade size** and **Closed PnL**
- Outliers filtered to ensure cleaner visuals and trends

---

##  Deliverables

-  Jupyter Notebooks (`notebook_1`, `notebook_2`)
-  Visualizations saved in `/outputs`
-  Merged dataset and source files in `/csv_files`
-  Final report (`ds_report.pdf`)
-  GitHub repository with structured README

---

## 🛠️ Tools Used

- **Python**: pandas, matplotlib, seaborn
- **Jupyter Notebooks / Google Colab**
- **Git & GitHub**

---

 *This project demonstrates the link between market psychology and trader performance.*  
 For questions or review: **Saloni1999-star**

 
