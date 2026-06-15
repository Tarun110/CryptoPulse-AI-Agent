# 🤖 CryptoPulse AI Agent

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![CrewAI](https://img.shields.io/badge/CrewAI-6E40C9?style=flat-square)
![Groq](https://img.shields.io/badge/Groq-F55036?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

**LLM-powered cryptocurrency market research agent** — autonomous news analysis, price signal extraction, and structured report generation using CrewAI, Groq, Exa Search, and Alpha Vantage.

</div>

---

## What It Does

CryptoPulse is a multi-agent AI system that autonomously researches a cryptocurrency, synthesizes live news and price data, and generates a structured investment research report — without manual prompting.

**The agent pipeline:**
1. **News Agent** — queries Exa Search for the latest crypto news and sentiment signals
2. **Price Agent** — fetches OHLCV data from Alpha Vantage and identifies trend patterns
3. **Analyst Agent** — synthesizes both sources into a structured markdown report with risk/opportunity highlights

---

## Key Results

- End-to-end research report generated in under 60 seconds per asset
- Covers: sentiment summary, price trend analysis, key risk factors, outlook
- Modular architecture — swap any data source or model without rewiring the pipeline

---

## Architecture

```
User Input (ticker symbol)
        │
        ▼
┌───────────────────────────────────┐
│         CrewAI Orchestrator       │
├──────────────┬────────────────────┤
│  News Agent  │   Price Agent      │
│  (Exa Search)│ (Alpha Vantage)    │
└──────────────┴────────────────────┘
        │               │
        └──────┬─────────┘
               ▼
       Analyst Agent (Groq LLM)
               │
               ▼
     Structured Research Report
```

---

## Tech Stack

| Component | Tool |
|---|---|
| Agent Framework | CrewAI |
| LLM | Groq (Llama 3) |
| News Retrieval | Exa Search API |
| Price Data | Alpha Vantage API |
| Language | Python 3.10+ |

---

## Setup & Run

```bash
# 1. Clone the repo
git clone https://github.com/Tarun110/CryptoPulse-AI-Agent.git
cd CryptoPulse-AI-Agent

# 2. Install dependencies
pip install -r requirements.txt

# 3. Set your API keys
cp .env.example .env
# Fill in: GROQ_API_KEY, EXA_API_KEY, ALPHA_VANTAGE_API_KEY

# 4. Run
python main.py
```

---

## Sample Output

```
=== CryptoPulse Report: BTC ===
Date: 2025-01-15

SENTIMENT: Moderately Bullish
Recent news highlights ETF inflow momentum and positive macro signals.

PRICE TREND: Uptrend (7-day), resistance at $98,200
Volume: Above 30-day average (+18%)

RISK FACTORS:
- Regulatory news from SEC pending
- Altcoin rotation risk

OUTLOOK: Cautiously positive short-term. Watch $94K support level.
```

---

## Project Structure

```
CryptoPulse-AI-Agent/
├── agents/
│   ├── news_agent.py
│   ├── price_agent.py
│   └── analyst_agent.py
├── tools/
│   ├── exa_search.py
│   └── alpha_vantage.py
├── main.py
├── requirements.txt
└── .env.example
```

---

## Author

**Tarun Sai Reddy Kummetha** — [LinkedIn](https://www.linkedin.com/in/tarun-sai-reddy-k-3182b2237) · [Portfolio](https://tarun110.github.io/tarunreddy.github.io/)
