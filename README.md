# LLM AI Bootcamp Materials

Hands-on labs for building with large language models: API usage, multimodal apps, open-source tooling, retrieval-augmented generation, structured outputs, fine-tuning, and agentic workflows. Content is organized as **numbered modules**, each with Jupyter notebooks and, in some cases, exported workflow files.

## What this course covers

- **Foundations** — OpenAI-style chat APIs, system prompts, and safe handling of secrets via `.env` (never commit API keys).
- **Multimodal & UX** — Vision use cases (e.g., image-based calorie tracking) and interactive UIs with **Gradio**, including streaming-style patterns.
- **Comparison & ecosystem** — Benchmarking multiple providers (e.g., OpenAI, Claude, Gemini) on the same task; **Hugging Face** for open models, document Q&A, and reasoning / leaderboard exploration.
- **Production-minded patterns** — **RAG** with **LangChain**, **Pydantic** for validated structured outputs across models.
- **Customization** — **PEFT / LoRA** fine-tuning of open-source LLMs (labs that expect **GPU**; notebooks point to **Google Colab** where needed).
- **Agents & orchestration** — **AutoGen** (multi-model teams), **LangGraph** (agentic workflows, e.g., a travel-agent style lab), **CrewAI** (including data-science automation), **n8n** (importable JSON workflows), and **MCP** with the **OpenAI Agents SDK**.

## Module map

| Module | Focus | Main artifacts |
|--------|--------|----------------|
| 0 | Course introduction | Sample data (`Financial_Statement.csv`) |
| 1 | Text / ChatGPT API | `Build a Character AI Chatbot Using OpenAI API.ipynb` |
| 2 | Vision | `Build a Calorie Tracker.ipynb` |
| 3 | Gradio & streaming | `An Adaptive LLM-Based AI Tutor with Gradio Interface for Multi-Level Learning.ipynb` |
| 4 | Multi-model benchmarking | `Landing Page Generator with OpenAI, Claude, and Gemini.ipynb` |
| 5 | Hugging Face (1) | `Chat_with_Documents_Using_Hugging_Face_Open_source_LLMs.ipynb` |
| 6 | Hugging Face (2) | `Reasoning_LLMs_in_Hugging_Face_&_LeaderBoards.ipynb` |
| 7 | RAG & LangChain | `RAG & LangChain Lab - Ask Eleven Madison Park Restaurant.ipynb` |
| 8 | Structured outputs | `Build a resume AI assistant with OpenAI, Gemini, & Pydantic.ipynb` |
| 9 | Fine-tuning | `Open_Source_LLM_Fine_Tuning_Using_PEFT_LORA.ipynb` |
| 10 | AutoGen | `Building Interactive Multi-Model AI Agent Teams with AutoGen.ipynb` |
| 11 | LangGraph | `Build Agentic AI Workflows Using LangGraph.ipynb` |
| 12 | CrewAI | `Automating Data Science with CrewAI Agents.ipynb`, `Predictive Analytics Using Machine Learning.ipynb`, `notebookExecutor.py` |
| 13 | n8n agents | Numbered `*.json` workflow exports (summarization, tools, sheets, triggers, etc.) |
| 14 | MCP | `MCP Server.ipynb`, `Build an AI Tutor Using MCP and OpenAI Agents SDK.ipynb` |

## Getting started

1. **Python environment** — Use **Anaconda** or another Python 3.x setup with **Jupyter** (or **VS Code / Cursor** with a Jupyter kernel). Module 1’s notebook walks through Anaconda if you are new to it.
2. **Install dependencies** — Each notebook lists its own imports; install packages as you open each lab (e.g., `openai`, `python-dotenv`, `gradio`, `langchain`, etc.).
3. **API keys** — Create a `.env` file in the project (or next to the notebook, per lab instructions) for provider keys. This repository’s `.gitignore` excludes `.env` and common secrets patterns; do not commit keys or paste them into notebooks.

## Notes

- **GPU / Colab** — Several Hugging Face and fine-tuning notebooks state that they need **GPU** access; they include **Colab** links inside the notebook for that path.
- **Generated outputs** — Some folders contain HTML or other outputs from runs (e.g., landing-page HTML); treat them as examples, not source of truth.
- **n8n** — Module 13 is primarily **workflow JSON** files meant to be imported into **n8n**, not Python notebooks.

This repo is **educational lab material**: run cells in order, complete the “practice opportunity” sections where provided, and adjust models or providers to match your accounts and budget.
