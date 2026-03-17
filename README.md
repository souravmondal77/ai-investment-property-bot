# 🧠 AI Investment Property Bot

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![LangChain](https://img.shields.io/badge/LangChain-LLM-yellow)
![CrewAI](https://img.shields.io/badge/CrewAI-Agents-green)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

An AI-powered system that uses LLM agents to research, analyze, and generate insights on real estate investment opportunities.

---

## 📌 Table of Contents

- [🚀 Features](#-features)
- [🛠️ Tech Stack](#️-tech-stack)
- [📦 Installation](#-installation)
- [▶️ Usage](#️-usage)
- [⚠️ Common Errors & Fixes](#️-common-errors--fixes)
- [📁 Project Structure](#-project-structure)
- [🎯 Roadmap](#-roadmap)
- [👨‍💻 Author](#-author)

---

## 🚀 Features

- 🔍 Automated property research
- 📊 Market trend analysis
- 🤖 Multi-agent collaboration using CrewAI
- 🧾 AI-generated investment reports
- 🏠 Local LLM support via Ollama

---

## 🛠️ Tech Stack

| Technology  | Purpose |
|------------|--------|
| Python     | Core programming language |
| LangChain  | LLM integration |
| CrewAI     | Multi-agent orchestration |
| Ollama     | Local LLM execution |

---

## 📦 Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/ai-investment-property.git
cd ai-investment-property
```

---

### 2️⃣ Create a Virtual Environment

```bash
conda create -n crew python=3.11
conda activate crew
```

---

### 3️⃣ Install Dependencies

```bash
pip install "crewai[tools]"
pip install langchain-community
pip install ollama
```

---

### 4️⃣ Install Ollama & Model

```bash
ollama pull openhermes
```

---

### 5️⃣ Setup API Key

Update your code:

```python
import os
os.environ["SERPER_API_KEY"] = "your_api_key_here"
```

---

### 6️⃣ Run the Project

```bash
python main.py
```

---

## ▶️ Usage

Run the script and the AI agents will:

- Research top investment suburbs in Sydney  
- Analyze pricing, rental yield, and trends  
- Generate a structured investment report  

---

## ⚠️ Common Errors & Fixes

### ❌ Model not found: openhermes

```bash
ollama pull openhermes
```

---

### ❌ Deprecation Warning (LangChain)

Install updated package:

```bash
pip install -U langchain-ollama
```

Then update import:

```python
from langchain_ollama import OllamaLLM
```

---

### ❌ Invalid verbose value

Fix:

```python
verbose=True
```

---

## 🧠 Project Overview

This project uses CrewAI to build a multi-agent system for property research:

- Research Agent → Finds promising suburbs  
- Writer Agent → Summarizes insights  
- Ollama → Runs local LLM  
- Serper → Enables web search  

---

## 👨‍💻 Author

**Sourav Mondal**

---

## 🔗 Other References

- CrewAI documentation  