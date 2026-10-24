# LangGraph: Build Stateful Agentic AI Chatbots

An Agentic AI application built with **LangGraph, Groq, and Streamlit** that allows users to interact with a large language model through a chat interface.

## Project Overview

This project demonstrates how to build an LLM-powered chatbot application using LangGraph for workflow orchestration, Groq for language model inference, and Streamlit for the user interface.

Users can select the available model and use case, enter a question, and view the generated response through the application.

## Tech Stack

- **Python** — Application development
- **Streamlit** — Interactive web interface
- **LangGraph** — Graph-based workflow orchestration
- **Groq** — Hosted LLM inference
- **LangChain Groq** — Integration with Groq models

## Application Workflow

1. Load the Streamlit interface.
2. Read the selected LLM and use-case configuration.
3. Initialize the selected Groq language model.
4. Build the LangGraph workflow for the selected use case.
5. Process the user's message through the configured graph.
6. Display the response in the Streamlit interface.

## Project Structure

```text
Agentic-AI/
├── app.py
├── requirements.txt
└── src/
    └── langgraphagenticai/
        ├── main.py
        ├── LLMS/
        │   └── groqllm.py
        ├── graph/
        │   └── graph_builder.py
        └── ui/
            ├── uiconfigfile.ini
            ├── uiconfigfile.py
            └── streamlitui/
                ├── loadui.py
                └── display_result.py
```

*Note: This structure lists the files identified so far. Keep any additional folders and files that exist in your repository.*

## Prerequisites

- Python 3.11 or a compatible version
- A Groq API key
- Git

## Installation

Clone the repository:

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd <YOUR_PROJECT_FOLDER>
```

Create and activate a virtual environment.

**Windows PowerShell:**

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

Install dependencies:

```powershell
python -m pip install -r requirements.txt
```

## Environment Configuration

Set your Groq API key as an environment variable or configure it using the environment-variable method expected by the application.

For example, in PowerShell:

```powershell
$env:GROQ_API_KEY = "your_groq_api_key"
```

Replace the placeholder with your own key. Never commit API keys, passwords, or other secrets to GitHub.

## Run the Application

From the project root, execute:

```powershell
python -m streamlit run app.py
```

Open the local URL displayed in your terminal.

## Key Learning Objectives

- Building an LLM-powered chat application
- Integrating Groq-hosted language models
- Creating graph-based workflows with LangGraph
- Developing interactive applications with Streamlit
- Organizing an AI project into separate UI, LLM, and graph modules

## Current Scope

The repository code should be reviewed to confirm the exact graph nodes, state management, supported use cases, and any tool-calling capabilities before describing those features as implemented.

This project currently demonstrates an LLM application workflow. It should not be described as a custom-trained model or a RAG system unless those capabilities are implemented in the code.

## Future Improvements

- Add additional use cases and graph workflows.
- Implement conversation history and state persistence.
- Add input validation and improved error handling.
- Add automated tests.
- Deploy the application to a hosting platform.

## Author

**Your Name**

AI Engineering | Generative AI | LangGraph | LLM Applications
