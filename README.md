
# Agno Agent Suite 🤖

A comprehensive suite of intelligent AI agents built using the [Agno framework](https://github.com/agno-ai/agno). This repository serves as an enterprise-grade toolkit showcasing various multi-agent workflows, contextual memory, and specialized tools.

## 🌟 Features & Agents

This toolkit includes several ready-to-use agents:

*   **📈 Financial Analyst (`finance.py`)**: An investment analyst agent that researches stock prices, analyst recommendations, and stock fundamentals using `YFinanceTools` and `DuckDuckGoTools`.
*   **🎥 YouTube Video Analyzer (`youtube_analyzer.py` & `ui.py`)**: A Streamlit-based web application that analyzes YouTube videos, creates timestamps, and summarizes educational, technical, or creative content.
*   **🌍 Multilingual Translation Team (`team.py`)**: A multi-agent team comprising English, Chinese, and Hindi agents that collaborate to answer user queries in multiple languages simultaneously.
*   **🧠 Cognitive Memory Agent (`memory.py`)**: An agent with persistent memory capabilities (using `SqliteDb`) that can remember user details across sessions.

## 🚀 Tech Stack

*   **Framework**: Agno
*   **Models used**: 
    *   Groq (`qwen/qwen3-32b`)
    *   OpenAI (`gpt-5.2`)
*   **UI**: Streamlit
*   **Tools/Integrations**: Yahoo Finance, DuckDuckGo, YouTube Tools, SQLite

## ⚙️ Setup & Installation

1. Clone the repository.
2. Install the required dependencies:
   ```bash
   pip install agno streamlit python-dotenv groq yfinance duckduckgo-search rich
   ```
3. Set up your environment variables by creating a `.env` file:
   ```env
   GROQ_API_KEY=your_groq_api_key
   OPENAI_API_KEY=your_openai_api_key
   ```
4. Run individual agents using python (e.g., `python finance.py`) or start the Streamlit UI:
   ```bash
   streamlit run ui.py
   ```
