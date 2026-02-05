
 Trader Performance vs Market Sentiment
Primetrade.ai – Data Science / Analytics Intern

This project analyzes how Bitcoin market sentiment (Fear vs Greed) relates to trader behavior and performance on the Hyperliquid platform. The objective is to uncover actionable insights that can help inform smarter, sentiment-aware trading strategies.

 Project Structure

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

---

 Setup and How to Run

 Step 1: Clone the repository
bash
git clone https://github.com/<your-username>/trader-sentiment-analysis.git
cd trader-sentiment-analysis


 Step 2: Install required libraries

bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter


Step 3: Run the notebook


jupiter notebook notebook.ipynb


All charts and tables will be generated automatically and saved in the `outputs/` directory.


 Output Charts and Tables

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


 Methodology

1. Loaded Bitcoin Fear/Greed sentiment data and Hyperliquid historical trader data
2. Cleaned datasets by removing duplicates and handling missing values
3. Parsed timestamps and aligned both datasets at a daily level
4. Engineered key metrics including daily PnL, trades per day, average leverage, trade size, and long/short ratio
5. Analyzed performance differences across Fear and Greed sentiment regimes
6. Segmented traders based on leverage and trading frequency
7. (Bonus) Built a simple logistic regression model to predict daily profitability using sentiment and behavioral features



Key Insights

* Trading performance is more volatile during Fear days, indicating emotionally driven and reactive trading behavior
* High-leverage traders tend to underperform during Greed periods due to overconfidence and crowd-following behavior
* Frequent traders adapt better during Fear regimes by capturing short-term market volatility



Strategy Recommendations

1. Reduce leverage exposure during Greed days, especially for high-leverage traders, to limit downside risk
2. Allow disciplined and consistent traders to increase trade frequency during Fear days to take advantage of volatility


