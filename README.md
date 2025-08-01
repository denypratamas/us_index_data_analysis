# 📊 QQQ vs SPY: Finding the Optimal Portfolio Composition

Welcome to this data-driven project where we compare **QQQ (Nasdaq-100 ETF)** vs **SPY (S&P 500 ETF)** to determine the **optimal portfolio allocation** based on historical performance metrics.

---

## 🧠 Objective

The main goal is to analyze and compare the performance of QQQ and SPY over time, using key quantitative metrics, and determine which portfolio composition offers the best **risk-adjusted return**.

---

## 📥 Data Source

- Data is fetched using [`yfinance`](https://github.com/ranaroussi/yfinance)
- Timeframe: 10 Years starting from January 1, 2015 to July 21, 2025
- Assets analyzed:  
  - **QQQ** – Invesco QQQ Trust (Nasdaq-100)  
  - **SPY** – SPDR S&P 500 ETF Trust

---

## 📈 Metrics Used

To evaluate and compare performance, the following metrics were calculated:

- **CAGR** (Compound Annual Growth Rate)
- **Sharpe Ratio** – risk-adjusted return vs volatility
- **Sortino Ratio** – downside risk-adjusted return
- **Calmar Ratio** – return vs drawdown
- **Max Drawdown** – peak-to-trough loss
- **Total Return** – overall growth over the period
- **Rolling Returns** – performance over rolling windows
- **Rolling Return 1 Year** – annualized performance over 1-year windows

All metrics are normalized to ensure fair comparison across mixed scales.

---

## 🛠️ Methodology

1. Collected historical adjusted close prices using `yfinance`
2. Basic data cleaning and preprocessing
3. Basic Exploratory Data Analysis (EDA) to visualize trends
4. Calculated daily returns and derived performance metrics
5. Created a **composite score** combining Sharpe, Sortino, Calmar, and Max Drawdown
6. Iterated through portfolio weight combinations (e.g. 0–100% QQQ, 100–0% SPY)
7. Identified the best portfolio allocation based on composite score

---

## ✅ Result

The portfolio with the **best overall risk-return profile** (based on composite score) is:
- **QQQ**: 57%
- **SPY**: 43%
This allocation provides a balanced exposure to both indices, optimizing for risk-adjusted returns.


---

## 🙋‍♂️ For Beginners

> If you're new to investing or portfolio analysis, don't stress — this project walks through the full breakdown of metrics and logic step-by-step in each notebook. You’ll learn how to evaluate assets beyond just “which one went up more.”

---

## ⚠️ Disclaimer

> This project is for **educational purposes only**.  
> **Not financial advice (NFA)**.  
> Always **do your own research (DYOR)** before making investment decisions.

---

## 🚀 Tools & Libraries

- Python 3.10+
- [yfinance](https://pypi.org/project/yfinance/)
- pandas, numpy, matplotlib, seaborn, scikit-learn
- Jupyter Notebook for interactive analysis

---

## 👨‍💻 Author

Built with passion by a data and finance enthusiast.  
Feel free to fork or star ⭐ if you found this useful!