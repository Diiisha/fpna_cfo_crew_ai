# 🤖 FP&A CFO Crew AI

> **A production-ready Multi-Agent AI application demonstrating AI workflow orchestration, LLM integration, and intelligent automation using CrewAI, FastAPI, and Streamlit.**

## 📌 Overview

This project demonstrates how multiple specialized AI agents collaborate to solve complex business workflows using Large Language Models (LLMs).

Although the implementation uses **Financial Planning & Analysis (FP&A)** as its use case, the underlying architecture is designed to be reusable across multiple domains such as customer support, healthcare, HR, operations, and enterprise automation.

## ✨ Key Highlights

- 🤖 Multi-Agent architecture built with CrewAI
- 🧠 LLM-powered task orchestration
- ⚡ FastAPI backend
- 📊 Interactive Streamlit dashboard
- 🗄️ Structured data integration
- 🔄 Modular and scalable architecture
- 🧩 Easily adaptable to different business domains

## 🛠 Tech Stack

- Python
- CrewAI
- FastAPI
- Streamlit
- PostgreSQL
- DuckDB
- OpenAI / LLM APIs


---

## 🏗️ High-Level Architecture

```text
                         User
                           │
                           ▼
                  Streamlit Dashboard
                           │
                           ▼
                    FastAPI Backend
                           │
                           ▼
              CrewAI Multi-Agent System
                           │
        ┌──────────────────┼──────────────────┐
        ▼                  ▼                  ▼
 Data Connector      FP&A Analyst      CFO Copilot
        │                  │                  │
        └──────────────────┼──────────────────┘
                           ▼
                 OpenAI / Gemini LLM
                           │
                           ▼
              Business Insights & Reports
```

## Agents

### 🔗 Data Connector Agent
Responsible for collecting and preparing structured business data from multiple sources before it is processed by other AI agents.

**Responsibilities**
- Integrates structured datasets
- Cleans and prepares business data
- Provides consistent inputs for downstream agents

---

### 📊 FP&A Analyst Agent
Analyzes financial and operational data to generate forecasts, identify trends, and perform variance analysis.

**Responsibilities**
- Forecasting
- Variance analysis
- Financial performance evaluation
- Business insight generation

---

### 📈 Profit Twin Agent
Performs scenario analysis to evaluate how different business decisions affect profitability and operational performance.

**Responsibilities**
- Scenario simulation
- Profitability analysis
- Impact assessment

---

### 👨‍💼 CFO Copilot Agent
Summarizes outputs from all agents into concise executive-level insights for decision-makers.

**Responsibilities**
- Executive summaries
- Recommendation generation
- Business reporting

## Setup

## ⚙️ Setup

### Prerequisites

Before running the project, ensure you have:

- Python 3.10+
- Git
- OpenAI API Key (or compatible LLM provider)

---

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Diiisha/fpna_cfo_crew_ai.git
cd fpna_cfo_crew_ai
```

---

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 3️⃣ Configure Environment Variables

Create a `.env` file:

```env
OPENAI_API_KEY=your_api_key
```

---

### 4️⃣ Run the Application

```bash
streamlit run dashboards/fpna_dashboard.py
```

## Project Structure

```text
fpna_cfo_crew_ai/
│
├── dashboards/          # Streamlit user interface
├── data/                # Sample datasets and processed data
├── prompts/             # Prompt templates used by AI agents
├── tasks/               # Agent task definitions and workflows
├── utils/               # Shared helper functions and utilities
├── api_server.py        # FastAPI backend service
├── app.py               # Application entry point
├── requirements.txt     # Project dependencies
├── .env.example         # Environment variable template
└── README.md            # Project documentation
```

### Folder Overview

| Folder | Purpose |
|--------|---------|
| **dashboards/** | Interactive Streamlit interface |
| **data/** | Stores datasets used by the application |
| **prompts/** | Contains prompt templates for AI agents |
| **tasks/** | Defines agent workflows and execution logic |
| **utils/** | Shared utility modules across the project |


