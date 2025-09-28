# GEMINI.md

## Project Overview

This project is a Python application that utilizes the `langchain` library to create a conversational AI agent. The agent is built using the ReAct (Reasoning and Acting) framework, which allows it to reason about a user's query and use tools to find information.

The primary technologies used are:
- **Python:** The core programming language.
- **LangChain:** A framework for developing applications powered by large language models (LLMs).
- **OpenAI:** The LLM provider used for the agent's intelligence.
- **Tavily:** A search tool that the agent can use to find information on the internet.
- **Pydantic:** A library for data validation and settings management.

The project is structured as follows:
- `main.py`: The main entry point for the application. It creates the agent, defines the tools, and runs the main logic.
- `prompt.py`: Contains the prompt template for the ReAct agent.
- `schemas.py`: Defines the data schemas for the agent's response and sources.
- `pyproject.toml`: The project's configuration file, which includes the dependencies.

## Building and Running

To run this project, you will need to have Python 3.11 or higher installed. You will also need to install the dependencies listed in the `pyproject.toml` file.

**1. Install Dependencies:**

```bash
pip install -r requirements.txt
```

**2. Set up Environment Variables:**

The project uses an `.env` file to manage environment variables. You will need to create a `.env` file in the root of the project and add the following:

```
OPENAI_API_KEY="your-openai-api-key"
TAVILY_API_KEY="your-tavily-api-key"
```

**3. Run the Application:**

To run the application, execute the `main.py` file:

```bash
python main.py
```

## Development Conventions

- **Dependency Management:** The project uses `pyproject.toml` to manage dependencies.
- **Code Style:** The project uses `black` for code formatting and `isort` for import sorting.
- **Type Hinting:** The project uses type hints for all function signatures and variables.
- **Data Validation:** The project uses `pydantic` to define data schemas and validate data.
