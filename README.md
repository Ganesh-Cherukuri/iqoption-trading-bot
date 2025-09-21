# IQ Option Trading Bot

## 📌 Overview
This project is a fully functional **trading bot** built for the **IQ Option platform**.  
The bot can connect to the IQ Option API, fetch market data, place trades, and manage risk with stop-loss rules.  
It is designed to work first with **demo accounts** for testing, and can later be connected to a **real account**.

---

## ⚙️ Features
- ✅ Connects securely to IQ Option (Demo & Real Accounts).  
- ✅ Fetches all available **binary options, forex, and stock assets**.  
- ✅ Places trades automatically based on rule-based filters.  
- ✅ Includes **stop-loss protection** to minimize risk.  
- ✅ Supports **different time zones** for trading.  
- ✅ Stores trading data in **Supabase database** (for history & analysis).  
- ✅ Collects live market data during trading.  
- ✅ Designed to integrate **predictive AI models** in the future.  

---

## 🏗️ Architecture
The bot follows a modular design:

1. **Data Collection Layer**  
   - Fetches live market data from IQ Option API.  
   - Collects and stores trade details in Supabase.  

2. **Rule-Based Strategy Layer**  
   - Applies filters (like asset availability, time zone, stop-loss).  
   - Makes trade entry/exit decisions.  

3. **(Future) AI Predictive Layer**  
   - Train ML models on historical market data.  
   - Predict profitable assets before trading.  

4. **Execution Layer**  
   - Places buy/sell trades on IQ Option.  
   - Manages active trades.  

---

## 🚀 How to Run
1. Install dependencies:
   ```bash
   pip install iqoptionapi supabase
