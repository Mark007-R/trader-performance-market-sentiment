# Trader Performance vs Market Sentiment (Fear & Greed Analysis)

## Overview
In this project, I analyzed how Bitcoin market sentiment influences trader behavior
and performance using historical trade data from Hyperliquid and the Bitcoin
Fear & Greed Index.

Instead of focusing on price prediction, the goal of this analysis was to understand
how different sentiment regimes (Fear vs Greed) affect profitability, risk-taking,
and trading consistency.

---

## Datasets Used

### 1. Bitcoin Fear & Greed Index
- Date
- Sentiment classification (Extreme Fear, Fear, Neutral, Greed, Extreme Greed)
- Sentiment score

### 2. Historical Trader Data (Hyperliquid)
- Trade timestamp
- Buy/Sell side
- Trade size (USD)
- Closed PnL
- Account-level trading activity

---

## Approach & Methodology
- Cleaned and preprocessed both datasets
- Mapped daily market sentiment to individual trades based on trade date
- Grouped sentiment into broader Fear and Greed regimes
- Analyzed trader performance using metrics such as:
  - Average PnL
  - Win rate
  - PnL distribution
  - Cumulative PnL over time
- Visualized performance differences across sentiment regimes for interpretability

The analysis focuses on exploratory insights rather than complex modeling, prioritizing
clarity and real-world relevance.

---

## Key Insights

### 1. Trader performance changes across sentiment regimes
From my analysis, trader performance differs noticeably between Fear and Greed periods.
The impact of sentiment is not limited to returns alone, but also affects trading
behavior and consistency.

---

### 2. Greed leads to higher activity and higher volatility
During Greed periods, traders tend to trade more frequently and take on higher risk.
While some large profits occur, losses also increase significantly, resulting in
greater PnL volatility without a meaningful improvement in win rate.

---

### 3. Fear encourages more disciplined trading
Fear periods show more stable win rates and lower PnL variance.
Extreme losses are less frequent, suggesting more cautious position sizing and
selective trade execution.

---

### 4. Market sentiment is a contextual signal, not a predictor
I observed only a weak to moderate relationship between sentiment score and individual
trade profitability. Positive sentiment does not guarantee profits, and negative
sentiment does not consistently lead to losses.

This suggests that sentiment is better used as a **risk-management or regime signal**
rather than a direct buy/sell indicator.

---

### 5. Long-term performance is regime-dependent
Cumulative PnL trends diverge across sentiment regimes.
A strategy that performs well in one sentiment environment may underperform in another,
highlighting the importance of regime-aware analysis.

---

## Tools & Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## Conclusion
From this analysis, I found that market sentiment provides valuable context for
understanding trader behavior and managing risk.
Incorporating sentiment-aware controls can improve consistency and reduce downside risk,
even without relying on complex predictive models.

---

## Author
**Mark**
