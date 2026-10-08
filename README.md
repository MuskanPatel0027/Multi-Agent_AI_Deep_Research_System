# 🤖 Multi-Agent AI Deep Research System

An AI-powered research assistant that uses multiple specialized agents to **search the web, extract relevant information, generate a structured research report, and critically evaluate the final output**.

The system combines **LangChain agents, Groq LLMs, web search, web scraping, and Streamlit** into an automated research pipeline.

---

## 🚀 Features

* 🔎 **Search Agent** — searches the web for recent and relevant information.
* 🌐 **Reader Agent** — selects relevant sources and extracts deeper information from web pages.
* ✍️ **Writer Agent** — generates a structured and professional research report.
* 🧐 **Critic Agent** — evaluates the generated report and provides a score, strengths, and areas for improvement.
* 🔗 **Web Search & Scraping** — gathers information from external sources.
* 📑 **Structured Reports** — reports include:

  * Introduction
  * Key Findings
  * Conclusion
  * Sources
* 💬 **Streamlit UI** — provides an interactive interface for submitting research topics.
* ⚡ **Groq-powered LLM** — uses Groq for fast language-model inference.

---

## 🏗️ System Architecture

```text
                    User Research Topic
                            │
                            ▼
                    ┌───────────────┐
                    │ Search Agent  │
                    │  Web Search   │
                    └───────┬───────┘
                            │
                            ▼
                    ┌───────────────┐
                    │ Reader Agent  │
                    │ Web Scraping  │
                    └───────┬───────┘
                            │
                            ▼
                    ┌───────────────┐
                    │ Writer Chain  │
                    │ Report Writer │
                    └───────┬───────┘
                            │
                            ▼
                    ┌───────────────┐
                    │ Critic Chain  │
                    │ Report Review │
                    └───────┬───────┘
                            │
                            ▼
                    Final Research Report
```

---

## 🧠 How It Works

### 1. Search Agent

The Search Agent receives the user's research topic and searches for recent, reliable, and detailed information using the web-search tool.

### 2. Reader Agent

The Reader Agent analyzes the search results, identifies a relevant source, and scrapes the selected webpage for additional information.

### 3. Writer

The Writer combines the search results and scraped content to generate a detailed research report containing:

* Introduction
* Key Findings
* Conclusion
* Sources

### 4. Critic

The Critic reviews the generated report and provides:

* Score out of 10
* Strengths
* Areas to improve
* Overall verdict

This creates a simple **research → write → evaluate** feedback workflow.

---

## 🛠️ Tech Stack

| Technology     | Purpose                         |
| -------------- | ------------------------------- |
| Python         | Core programming language       |
| LangChain      | Agent and LLM orchestration     |
| Groq           | LLM inference                   |
| OpenAI GPT-OSS | Language model                  |
| Streamlit      | Web interface                   |
| BeautifulSoup  | Web scraping                    |
| Web Search     | Information retrieval           |
| python-dotenv  | Environment variable management |

---

## 📁 Project Structure

```text
Multi-Agent_AI_Deep_Research_System/
│
├── app.py
├── agents.py
├── pipeline.py
├── tools.py
├── requirements.txt
├── .python-version
├── .gitignore
│
├── src/
│   └── multi_agent_ai_research_sys_with_langchain/
│
└── README.md
```

### Main Files

**`app.py`**
Streamlit application and user interface.

**`agents.py`**
Defines the Search Agent, Reader Agent, Writer chain, and Critic chain.

**`tools.py`**
Contains the web search and webpage scraping tools.

**`pipeline.py`**
Coordinates the complete research workflow from search to final critique.

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/MuskanPatel0027/Multi-Agent_AI_Deep_Research_System.git
```

### 2. Navigate to the project

```bash
cd Multi-Agent_AI_Deep_Research_System
```

### 3. Create a virtual environment

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

Create a `.env` file in the project root:

```env
GROQ_API_KEY=your_groq_api_key
```

Do **not** commit your `.env` file to GitHub.

---

## ▶️ Run the Application

Start the Streamlit application:

```bash
streamlit run app.py
```

The application will open in your browser.

---

## 💡 Example Use Cases

The system can be used for researching topics such as:

* Artificial Intelligence
* Machine Learning
* Generative AI
* Technology trends
* Research topics
* Product comparisons
* Emerging technologies
* Current industry developments

Example:

```text
Research Topic:
"Latest developments in Generative AI"
```

The system searches for information, extracts relevant content, generates a report, and evaluates the report.

---

## 🎯 Key Learning Outcomes

This project demonstrates practical experience with:

* Multi-agent AI systems
* LLM orchestration
* LangChain agents
* Prompt engineering
* Web information retrieval
* Web scraping
* Automated research pipelines
* LLM-based report generation
* LLM output evaluation
* Streamlit application development
* Environment and API-key management

---

## 👩‍💻 Author

**Muskan Patel**

GitHub: [@MuskanPatel0027](https://github.com/MuskanPatel0027)

---
