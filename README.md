# AI-Powered-Customer-Support-Automation-System
Here is the exact raw Markdown text. You can copy everything inside this block and paste it directly into your `README.md` file. It includes all the `#` headers, `` for bold text, and ````` for the code blocks!

```markdown
# AI-Powered Customer Support Automation System

## Project Description
This project is an automated customer support system built using **LangGraph** and a local LLM (**Qwen 2.5** via **Ollama**). It classifies user intents, retrieves context via a simulated RAG pipeline, routes queries to specialized department agents, utilizes SQLite for conversational memory, and includes a **Human-in-the-Loop (HITL)** approval process for high-risk requests.

## Setup Instructions
1. Install **Python 3.10** or higher.
2. Install the required libraries using your terminal:
```bash
py -m pip install langgraph==0.2.28 langchain-ollama==0.1.3 rich==13.9.4 langgraph-checkpoint-sqlite==1.0.4

```

*(Note: If `py` is not recognized, use `python -m pip install...`)*

3. Install [Ollama](https://ollama.com/) and pull the required model:

```bash
ollama pull qwen2.5:3b

```

## How to Run

1. Ensure the **Ollama** application is open and running in the background.
2. Open your terminal in the project directory.
3. Execute the Python script:

```bash
python support_automation.py

```

4. The system will automatically process 5 demonstration queries.
5. **Human-in-the-Loop:** For Query 4 (Refund Request), the terminal will pause and display a red high-risk warning. Press `Enter` to simulate manager approval and resume the graph execution.
