

## Trader Performance vs Market Sentiment

**Primetrade.ai – Data Science / Analytics Intern**

This project analyzes how Bitcoin market sentiment (Fear vs Greed) relates to trader behavior and performance on the Hyperliquid platform. The objective is to uncover actionable insights that help inform smarter, sentiment-aware trading strategies.

---

## Project Structure

```
trader-sentiment-analysis/
│
├── notebook.ipynb
├── data/
│   ├── fear_greed_index.csv
│   └── historical_trades.csv
│
├── outputs/
│   ├── pnl_by_sentiment.png
│   ├── behavior_by_sentiment.png
│   └── segment_performance.png
│
└── README.md
```

---

## Setup and How to Run

### Step 1: Clone the repository

```bash
git clone https://github.com/<your-username>/trader-sentiment-analysis.git
cd trader-sentiment-analysis
```

### Step 2: Install required libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### Step 3: Run the notebook

```bash
jupyter notebook notebook.ipynb
```

All charts and tables are generated automatically and saved in the `outputs/` directory.

---

## Output Charts and Tables

The notebook generates and saves the following outputs:

* Comparison of average daily PnL during Fear vs Greed days
* Trader behavior analysis by sentiment:

  * trade frequency
  * average trade size
  * long/short ratio
* Performance comparison across trader segments:

  * high vs low leverage traders
  * frequent vs infrequent traders

All outputs are saved as image files for easy review.

---

## Methodology

* Loaded Bitcoin Fear/Greed sentiment data and Hyperliquid historical trader data
* Cleaned datasets by removing duplicates and handling missing values
* Parsed timestamps and aligned both datasets at a daily level
* Engineered key metrics including daily PnL, trades per day, average leverage, trade size, and long/short ratio
* Analyzed performance differences across Fear and Greed sentiment regimes
* Segmented traders based on leverage and trading frequency
* (Bonus) Built a simple logistic regression model to predict daily profitability using sentiment and behavioral features

---

## Key Insights

* Trading performance is more volatile during Fear days, indicating emotionally driven and reactive trading behavior
* High-leverage traders tend to underperform during Greed periods due to overconfidence and crowd-following behavior
* Frequent traders adapt better during Fear regimes by capturing short-term market volatility

---

## Strategy Recommendations

* Reduce leverage exposure during Greed days, especially for high-leverage traders, to limit downside risk
* Allow disciplined and consistent traders to increase trade frequency during Fear days to take advantage of volatility

---


