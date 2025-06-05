# 📈 Stock Prediction AI

## 🧠 Overview
This project uses AI to simulate and optimize short-term stock trades using a small bankroll (starting with $500 or less). It focuses on **daily price movement prediction** and **trade simulation** on **high-volatility stocks**, with the goal of compounding profit as fast as realistically possible.

The project:
- 💹 Predicts next-day stock movement (up/down)
- 🔄 Simulates buy/sell trades with a fake bankroll
- 🧪 Evaluates accuracy and bankroll growth
- 🧰 Uses open-source tools like `yfinance`, `ta`, and `xgboost`

---

## 🎯 Goal
Turn a small bankroll ($1–$500) into a larger amount by:
- Making daily trades based on AI predictions
- Compounding gains over time
- Testing models before applying to real or paper trades

---

## 💹 Focused Tickers (High Volatility Targets)
These stocks are selected for their **large daily swings** and **high liquidity**:
- 💥 `TSLA` – Tesla
- 🔁 `MARA` – Marathon Digital
- 💥 `COIN` – Coinbase
- 📈 `TQQQ` – 3x Leveraged Nasdaq ETF
- 📉 `SQQQ` – 3x Inverse Nasdaq ETF

---

## 🧰 Tech Stack & Tools
- 📦 `yfinance` – Historical stock data
- 🧪 `ta` – Technical indicators (RSI, EMA, etc.)
- 📦 `xgboost` – Classification model
- 🧰 `scikit-learn` – Training & evaluation
- 🔌 Alpaca API – (optional) for paper/live trading
- 💻 Cursor – Development environment
- 📊 WandB – Logging and visualizing model performance

---

## 🔒 Model Training Constraints
- 🔒 No future data allowed (no leakage)
- 🧪 Train on 80% of past data, test on last 20%
- 📏 All model decisions must simulate realistic scenarios
- ✅ Evaluate on accuracy, win/loss ratio, and bankroll growth

---

## 📂 Project Structure

```bash
stock_prediction_ai/
├── data/
│   ├── raw/         # Raw OHLCV stock data
│   └── processed/   # Feature-engineered datasets
├── models/          # Saved model files
├── notebooks/       # Jupyter or dev notebooks
├── scripts/
│   ├── fetch_data.py        # Pulls historical data
│   ├── train_model.py       # Trains AI model on features
│   ├── simulate_trades.py   # Simulates trades and logs bankroll
│   └── utils.py             # Shared helper functions
├── output/
│   └── logs/        # Bankroll tracking and trade logs
├── requirements.txt
└── README.md
```

---

## 🚀 Quick Start

### 1. 📦 Install dependencies
```bash
pip install -r requirements.txt
```

### 2. 📥 Fetch data
```bash
python scripts/fetch_data.py
```

### 3. 🧠 Train model
```bash
python scripts/train_model.py
```

### 4. 💸 Simulate trades
```bash
python scripts/simulate_trades.py
```

---

## 🧠 Future Goals
- Add Reddit/Twitter/news sentiment
- Expand to more stocks using volatility filters
- Deploy live trades via Alpaca paper account
- Build ensemble or stacked models
- Launch minimal frontend or mobile PWA dashboard

---

## 🧑‍💻 Maintained by
Stephen @ TechWorksAZ | Built in Cursor IDE

# Stock Prediction Project

This project implements a machine learning-based stock prediction system using various technical indicators and historical data.

## Project Structure

```
stock_prediction/
├── data/
│   ├── raw/         # Raw stock data
│   └── processed/   # Processed and cleaned data
├── models/          # Trained models
├── notebooks/       # Jupyter notebooks for analysis
├── scripts/
│   └── fetch/       # Data fetching scripts
└── output/
    └── logs/        # Log files
```

## Setup

1. Clone the repository:
```bash
git clone https://github.com/techworksaz/stock_prediction.git
cd stock_prediction
```

2. Create and activate virtual environment:
```bash
python -m venv venv
# On Windows:
.\venv\Scripts\activate
# On Unix or MacOS:
source venv/bin/activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

[To be added as the project develops]

## License

[To be added]
