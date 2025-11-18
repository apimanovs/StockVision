# 📊 StockSense — Intelligent Stock Analytics Platform  
**Automated Fundamental Analysis • Real-Time Charts • Scoring Engine • Investment Verdicts**

StockSense is a modern, data-driven platform built to help investors quickly understand the quality of any publicly traded company.  
It automatically gathers financials, calculates key metrics, evaluates valuation & efficiency, and generates a simple final verdict:  
**Buy • Hold • Avoid.**

Designed for **individual investors**, **analysts**, and **engineers**, StockSense combines financial expertise with a clean technical architecture using **.NET, DDD, MediatR, PostgreSQL, and React**.

---

## 🚀 Features

### 🔍 1. **Ticker Search**
Enter any ticker — the system retrieves:
- current price  
- market capitalization  
- financial statements  
- valuation multiples  
- share structure  

---

### 📈 2. **Interactive Price Charts**
- historical price data  
- daily / weekly / monthly timeframes  
- TradingView chart integration (or equivalent)  

---

### 🧮 3. **Automated Fundamental Analysis**

#### **Growth**
- Revenue Growth  
- Net Income Growth  
- EPS Growth  
- Free Cash Flow  
- Operating Margin  

#### **Financial Health**
- Debt-to-Equity  
- Current Ratio  
- Interest Coverage  
- Cash vs Short-Term Debt  

#### **Valuation**
- P/E  
- P/S  
- P/B  
- EV / EBITDA  
- PEG  

#### **Efficiency**
- ROE  
- ROA  
- ROIC  

_All metrics are automatically calculated inside the internal **Metrics Engine**._

---

### 🏅 4. **Scoring Engine (0–100%)**

Companies are scored based on:
- fundamentals  
- debt levels  
- valuation fairness  
- growth dynamics  
- business efficiency  

| Score | Verdict |
|-------|---------|
| **75–100** | 🚀 Strong Buy / High Potential |
| **50–74**  | 🙂 Neutral / Hold |
| **0–49**   | 🛑 Avoid |

---

### ⭐ 5. **Favorites & Portfolio**
Save companies to:
- **Favorites**
- **My Portfolio**

---

### ⚔️ 6. **Company Comparison**
Compare **3–5 companies** side-by-side across all metrics.

---

### 📤 7. **Export**
Export analysis as:
- PDF  
- Excel  
- PNG snapshot  

---

## 🔌 Required Data Sources

To run the analysis, the backend expects the following financial data:

### **Pricing & Market Data**
- real-time price  
- historical candles  
- market cap  
- shares outstanding  

### **Financial Statements**
- Revenue (annual / TTM)  
- Net Income  
- EPS (annual / TTM)  
- EBIT / EBITDA  
- Cash  
- Total Debt / Short Debt  
- Total Equity  
- Free Cash Flow  
- CAPEX  

### **Multiples**
- P/E, P/S, P/B  
- ROE, ROA, ROIC  
- EV  
- EV/EBITDA  
- PEG  

---

## 🔌 Supported APIs

### **Free APIs**
- Financial Modeling Prep (FMP Free)  
- Twelve Data Free  
- Alpha Vantage  

### **Professional APIs**
- **Finnhub PRO** — best for fundamentals  
- **Twelve Data PRO** — excellent real-time pricing  
- **FMP Pro** — balanced and affordable  

**Recommended setup:** _Finnhub + Twelve Data._

---

## 🧱 Domain-Driven Design (DDD)

The solution is organized into independent layers:

### **Domain Layer**
- Entities  
- Value Objects  
- Domain Services  
- Domain Events  
- Business Rules  

### **Application Layer (CQRS + MediatR)**
- Commands  
- Queries  
- Handlers  
- Application Services  
- Orchestrates domain logic  

### **Infrastructure Layer**
- External API providers (Finnhub, FMP, TwelveData)  
- Entity Framework Core  
- PostgreSQL  
- Redis caching  
- Outbox pattern / background workers  

### **API Layer**
- REST endpoints  
- DTO mapping  
- Validation  
- (Optional) Authentication  

---

## 🖥 Frontend

- React (or Vue)  
- TradingView Advanced Chart Widget  
- TailwindCSS / Material UI  
- Responsive, mobile-friendly design  
- Comparison tables  
- Real-time price updates  

---

## 🧭 Roadmap

- [ ] Stock Screener (filters: price, P/E, ROE, debt, sector)  
- [ ] Portfolio analytics (risk, diversification, exposure)  
- [ ] Real-time alerts (rating change / volatility)  
- [ ] AI-based forward valuation (EPS forward, fair value model)  
- [ ] Telegram bot integration  
- [ ] OAuth + profiles + cloud sync  

---

## 📝 Summary

**StockSense** automatically analyzes US and EU stocks, calculates key metrics, visualizes price history, assigns a quality score, and provides a clear Buy/Hold/Avoid verdict.  
Built with a scalable and robust architecture using **.NET, DDD, MediatR, PostgreSQL, and React**, it is designed for investors and engineers who value reliability, clarity, and automation.

---
