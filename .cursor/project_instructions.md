# 📈 Stock Prediction AI – Project Instructions

**Project Name:** `Stock Prediction AI`  
**Primary Goal:**  
Use AI to grow a small bankroll ($1–$500) as quickly as possible using short-term daily stock trades.  
The model should predict **next-day price direction** on **high-volatility tickers** and simulate trades to track performance.

---

### 🧱 Project Structure
- `/data/`: raw and processed stock data  
- `/models/`: trained models  
- `/scripts/`: fetch, train, and simulate files  
- `/output/logs/`: bankroll logs

---

### 💹 Stock Targets
- `TSLA`, `MARA`, `COIN`, `TQQQ`, `SQQQ`

---

### 📦 Tools & Stack
- `yfinance`, `ta`, `xgboost`, `scikit-learn`, `wandb`, `Cursor IDE`

---

### 🔒 Constraints
- No future data leakage (chronological splits only)
- Train on past 80%, test on last 20%
- Use $500 fake bankroll, simulate 1 trade per day
- Daily prediction focus (no long-term investing)

---

### 🤖 AI Agent Prompts Should...
- Explain model logic and use meaningful filenames
- Reuse helpers from `scripts/utils.py` if available
- Ask for confirmation before overwriting anything
