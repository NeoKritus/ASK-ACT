# ASK&ACT — Agentic AI Orchestration & Specialized Multi-Agent Engine

ASK&ACT is an agentic AI platform that combines multiple specialized AI capabilities in one application. It supports code review, stock intelligence, market research, YouTube content analysis, and general AI conversation through modular AI workflows.

---

## Key Features

* **Multi-Agent Code Review Engine**: Analyzes submitted code through multiple specialized checks covering quality, correctness, security, performance, and testing.

* **Stock Intelligence**: Understands natural-language stock queries and coordinates relevant analysis to produce focused financial insights.

* **Market Data Analysis**: Retrieves market information and analyzes observable price, volume, and trend patterns for selected stocks.

* **Web & Social Intelligence**: Collects relevant online information to identify current discussions, trends, and market-related signals.

* **News Intelligence**: Processes recent company and market news to provide concise summaries, sentiment, and important developments.

* **YouTube Content Analysis**: Analyzes the content of YouTube videos and generates topic-focused insights and summaries.

* **General AI Chatbot**: Provides a conversational AI interface for general-purpose questions and interactions.

* **Multi-Agent Graph Workflows**: Uses graph-based orchestration to connect specialized processing stages and coordinate complex AI tasks.

---

## Why This Architecture?

* **Specialized AI Workflows**: Each major task has its own processing flow, making the system more focused than a single general-purpose AI agent.

* **Modular Design**: Independent agents, tools, and processing components can be extended without changing the entire application.

* **Privacy & Local AI Potential**: The architecture can use local open-source models to reduce external model dependency and keep sensitive processing closer to the user.

* **Modern Application Architecture**: A React frontend and FastAPI backend keep the user interface separate from the AI processing layer.

---

## System Architecture & Workflow (How It Works)

1. **User Input & Data Collection**: The user submits a question, code, stock query, or YouTube URL through the web interface.

2. **Specialized Processing**: The backend identifies the required workflow and coordinates the appropriate AI agents, tools, and data sources.

3. **Analysis & Synthesis**: Individual processing results are combined by the workflow to produce a unified response.

4. **Result Delivery**: The processed result is returned through the backend and displayed in the React interface.

---

## Agent Workflow Design

### Code Review

`Code → Multiple Specialized Checks → Result Evaluation → Final Review`

The code-review workflow separates different evaluation responsibilities before producing a consolidated result.

### Stock Intelligence

`User Query → Query Understanding → Relevant Analysis → Information Synthesis → Stock Insights`

The workflow determines the information required for the user's financial question before generating the response.

### YouTube Content Analysis

`YouTube URL → Content Retrieval → Topic Understanding → Analysis → Summary`

The system retrieves the video's underlying content and generates topic-focused information from it.

### General AI Chat

`User Message → AI Processing → Response`

A dedicated conversational workflow handles general-purpose user interactions.

---

## Tech Stack

| Domain               | Technologies                                   |
| :------------------- | :--------------------------------------------- |
| **Frontend**         | React, JavaScript, Tailwind CSS, Vite          |
| **Backend**          | Python, FastAPI, Uvicorn                       |
| **AI Orchestration** | LangGraph, LangChain                           |
| **AI Models**        | Local LLMs through Ollama / Open-Source Models |
| **Market Data**      | yfinance                                       |
| **Video Content**    | YouTube Transcript Retrieval                   |
| **Development**      | Git, GitHub, VS Code                           |

---

## Prerequisites

* Python 3.10+
* Node.js 18+
* npm
* Git
* Local Ollama runtime for the recommended local AI architecture
* Sufficient system resources for the selected local model
