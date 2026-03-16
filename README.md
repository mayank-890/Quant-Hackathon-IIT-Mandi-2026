# Quant Hackathon — IIT Mandi Xpecto 2026
## ML-Based Momentum Trading Strategy

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Event](https://img.shields.io/badge/Event-IIT%20Mandi%20Xpecto%202026-orange)

---

## Description

This project was developed for the **IIT Mandi Xpecto 2026 Quant Hackathon** (March 14, 2026).

It builds a machine learning-based long-only momentum trading strategy on a universe of 10 US large-cap stocks. Each week, the model predicts which stocks will generate a positive return over the next 7 days, selects the top 2, and holds an equal-weight portfolio with weekly rebalancing.

**Key highlights:**
- 14 engineered features (momentum, RSI, MACD, Bollinger Bands, ATR, volume)
- 3 ML models compared: Logistic Regression, Random Forest, XGBoost
- Strict train (2017–2022) / test (2023–2025) split — zero data leakage
- Realistic 0.1% transaction costs at entry and exit

---

## Stock Universe

AAPL · MSFT · GOOGL · AMZN · META · TSLA · JPM · V · JNJ · BRK-B

---

## Project Structure

```
quant-hackathon-iit-mandi-2026/
├── MayankSrivastava_QuantQuest_ESummit26.ipynb   ← Main notebook
├── QuantQuest_Report_MayankSrivastava.pdf     ← Full report
├── MayankSrivastava_QuantQuest_ESummit26_predictions.csv ← Weekly predictions
└── README.md
```

---

## Installation

**Step 1 — Clone the repository:**
```bash
git clone https://github.com/mayank-890/Quant-Hackathon-IIT-Mandi-2026.git
cd Quant-Hackathon-IIT-Mandi-2026
```

**Step 2 — Install required libraries:**
```bash
pip install pandas numpy scikit-learn xgboost yfinance matplotlib seaborn jupyter
```

---

## Usage

**Step 1 — Open the notebook:**
```bash
jupyter notebook MayankSrivastava_QuantQuest_ESummit26.ipynb
```

**Step 2 — Run all cells:**
```
Kernel → Restart & Run All
```

Data downloads automatically via yfinance — no manual file setup needed.

---

## Results (Test Period: 2023–2025)

| Metric | Value |
|--------|-------|
| Best Model | Logistic Regression |
| Sharpe Ratio | 1.2921 |
| Max Drawdown | -12.58% |
| Annualised Return | 33.11% |
| Hit Rate | 57.58% |

---

## Tech Stack

- **Python 3.10+**
- **pandas / numpy** — data processing
- **scikit-learn** — ML models
- **XGBoost** — gradient boosting
- **yfinance** — market data
- **matplotlib / seaborn** — visualisation

---

## Author

**Mayank Srivastava**
B.Tech — Computer Science & Engineering
IILM University, Greater Noida

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](www.linkedin.com/in/mayank-srivastava-490646365)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black)](https://github.com/mayank-890)

---

## Acknowledgements

Thanks to **IIT Mandi Xpecto '26** for organising the hackathon and providing a well-structured problem statement.

---

*Submitted for QuantQuest ESummit26 — Xpecto 2026, IIT Mandi | March 14, 2026*
