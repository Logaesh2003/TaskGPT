# TaskGPT

TaskGPT is a modular AI-powered application composed of three core services:

- **TaskGPT LLM** – Natural language processing and reasoning powered by LangChain, Groq/OpenAI.
- **TaskGPT UI** – Frontend interface built with Angular and Python integration.
- **TaskGPT DB** – Persistent storage layer using PostgreSQL.

All services communicate seamlessly through **FastAPI**, ensuring a robust, scalable, and traceable architecture.

---

## 🚀 Features

- **Modular Design**: Separate services for UI, LLM, and DB, organized as Git submodules.
- **AI Integration**: LangChain orchestration with Groq/OpenAI models for advanced task reasoning.
- **Modern Frontend**: Angular-based UI with Python backend hooks.
- **Reliable Storage**: PostgreSQL database with structured schema for task persistence.
- **FastAPI Communication**: Lightweight, high-performance API layer connecting all services.

---

## 🏗️ Architecture
+------------------+        +----------------+        +----------------+
|   TaskGPT UI     | <----> |   FastAPI Hub  | <----> |   TaskGPT LLM  |
| (Angular/Python) |        |                |        |   (LangChain)  |
+------------------+        +----------------+        +----------------+
        |                           |                         
        |                           v                         
        |                   +----------------+                 
        +------------------>|   TaskGPT DB   |
                            |  (PostgreSQL)  |
                            +----------------+


---

## 📂 Repository Structure
TaskGPT/
├── TaskGPT-UI/     # Angular + Python frontend
├── TaskGPT-LLM/    # LangChain + Groq/OpenAI service
├── TaskGPT-DB/     # PostgreSQL schema and DB service
└── .gitmodules     # Submodule definitions


