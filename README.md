# 🪙 CryptoPulse AI Agent: LLM-Powered Cryptocurrency Market Research using CrewAI, Groq & Exa

## 📌 Overview

Cryptocurrency markets are highly volatile and influenced by a combination of news events, market sentiment, historical price movements, and macroeconomic factors. Manually tracking crypto news, analyzing price trends, and preparing market summaries can be time-consuming and inconsistent.

This project builds an LLM-powered cryptocurrency research agent that uses a multi-agent AI workflow to analyze crypto market news, retrieve historical price data, and generate concise market reports. The system combines CrewAI agents, Groq-powered Llama 3 models, Exa Search, and Alpha Vantage price data to automate cryptocurrency research and analysis.

The project demonstrates an AI agent workflow including tool creation, API integration, LLM reasoning, news retrieval, historical price analysis, multi-agent collaboration, and automated report generation.

---

## 🚀 Key Features

### 🤖 Multi-Agent AI Workflow

Uses CrewAI to coordinate multiple specialized agents for cryptocurrency research and report generation.

Agents include:

- Customer Communicator
- Cryptocurrency News Analyst
- Cryptocurrency Price Analyst
- Cryptocurrency Report Writer

---

### 🔎 Cryptocurrency News Analysis

Retrieves cryptocurrency-related news using Exa Search.

Extracts article titles, URLs, publication dates, summaries, and relevant highlights.

Generates news-based market analysis and directional sentiment.

---

### 📈 Historical Price Analysis

Fetches daily cryptocurrency closing prices using Alpha Vantage API.

Analyzes recent price movement for selected crypto assets.

Supports ticker-based price lookup such as BTC, ETH, and other cryptocurrencies.

---

### 🧠 LLM-Powered Reasoning

Uses Groq API with Llama 3 for fast LLM inference.

Generates natural-language analysis from news and price data.

Combines multiple sources of information into a clear market report.

---

### 📝 Automated Report Generation

Creates a concise cryptocurrency market report using outputs from the news analyst and price analyst agents.

Provides an easy-to-understand summary of market trends and potential future direction.

---

## 🔧 Tech Stack

### Generative AI & Agents

- CrewAI
- LangChain
- Groq API
- Llama 3

### Search & Market Data

- Exa Search
- Alpha Vantage API
- DuckDuckGo Search

### Programming

- Python
- Pandas
- Requests

### Environment Management

- Python-dotenv

---

## 📂 Project Workflow

### 1️⃣ User Input

The system asks the user which cryptocurrency they want to research.

### 2️⃣ News Retrieval

The news analyst agent searches for recent cryptocurrency news using Exa Search.

### 3️⃣ Price Data Collection

The price analyst agent retrieves historical daily closing prices using Alpha Vantage.

### 4️⃣ News Analysis

The news analyst reviews recent market news and summarizes sentiment.

### 5️⃣ Price Analysis

The price analyst reviews historical prices and identifies short-term trend direction.

### 6️⃣ Report Writing

The report writer combines news analysis and price analysis into a final market summary.

### 7️⃣ Final Output

The system produces a concise cryptocurrency market report with a directional outlook.

---

## 🧪 Example Questions

What is the current market outlook for Bitcoin?

Analyze Ethereum based on recent news and price movement.

What is the short-term trend for BTC?

Summarize the latest cryptocurrency market sentiment.

Generate a market report for Solana.

Is Bitcoin likely to move up, down, or remain neutral?

---

## 📊 Agents Implemented

| Agent | Role |
|------|------|
| Customer Communicator | Collects the cryptocurrency ticker from the user |
| Cryptocurrency News Analyst | Retrieves and analyzes recent crypto news |
| Cryptocurrency Price Analyst | Analyzes historical price data |
| Cryptocurrency Report Writer | Generates the final market report |

---

## 📈 Key Insights

📌 Crypto market analysis benefits from combining both news sentiment and historical price movement.

📌 Multi-agent workflows help separate responsibilities such as user communication, news analysis, price analysis, and report writing.

📌 LLMs can transform raw market data into structured, easy-to-read summaries.

📌 External tools such as Exa and Alpha Vantage improve the usefulness of LLM applications by grounding responses in real-time data.

---

## 🏆 Skills Demonstrated

Generative AI

AI Agent Development

CrewAI

LangChain

Groq API

Llama 3

Tool Calling

API Integration

Cryptocurrency Market Analysis

Financial Data Analysis

Prompt Engineering

Python Development

Automated Report Generation

LLM Application Development

---

## 🎯 Business Value

Cryptocurrency research requires continuous monitoring of news, market sentiment, and price movement. This project automates the research process by combining AI agents, search tools, market data APIs, and LLM reasoning.

The system can help analysts, traders, researchers, and fintech teams quickly generate market summaries and identify emerging trends from multiple information sources.

---

## ⚠️ Disclaimer

This project is built for educational and portfolio purposes only. It does not provide financial advice, investment recommendations, or trading signals. Cryptocurrency markets are highly volatile, and all outputs should be independently verified before making financial decisions.
