## 🧩 n8n

- Type: Workflow automation platform
- What it does:
    Connects APIs, databases, and services through visual workflows — like an open-source Zapier.
    Use in AI stack:
    Automates data ingestion, triggers actions (e.g., “when document uploaded → embed → store → notify”), and exposes webhooks/tools for agents to call.

#### 🔁 Alternatives:

- 🧠 LangFuse Automations – purpose-built for LLM observability + automation.
- ⚙️ Apache Airflow – heavy-duty data/workflow orchestration (Python-based).
- 🪢 Temporal.io – code-first workflow engine, great for long-running AI tasks.
- 💬 Zapier / Make (Integromat) – SaaS-based no-code options for simpler integrations.

## 🧠 LangChain

- Type: AI orchestration & reasoning framework
- What it does:
Provides structure for building LLM-powered applications — handles prompts, memory, tools, agents, and retrieval.
Use in AI stack:
Acts as the “brain” that connects the model (Ollama) with tools (n8n, Pinecone, APIs).

#### 🔁 Alternatives:

- 🧩 LlamaIndex – more retrieval-centric (RAG pipelines, document loaders).
- ⚡ Semantic Kernel (Microsoft) – C#/Python SDK for planning & orchestration.
- 🪞 Haystack (deepset) – great for RAG, search, and QA pipelines.
- 🪄 CrewAI / AutoGen – agent frameworks for multi-agent or autonomous workflows.

## 🦙 Ollama

- Type: Local LLM model server
- What it does:
Runs large language models (like Llama 3, Mistral, Qwen) locally through an HTTP API.
Use in AI stack:
Provides the actual intelligence — LangChain sends prompts here to get responses or embeddings.

#### 🔁 Alternatives:

- 🧰 LM Studio – desktop LLM runner with UI, similar local model hosting.
- ⚙️ vLLM / TGI / OpenAI-Compatible servers – optimized inference engines for  custom hosting.
- 🧠 OpenAI / Anthropic / Claude / Gemini APIs – cloud-hosted LLMs with better reasoning & context.
- 🧩 Hugging Face Text Generation Inference (TGI) – scalable open-source LLM serving backend.

## 🪵 PineconeDB

- Type: Managed vector database
- What it does:
Stores vector embeddings (numerical representations of text) for fast similarity search.
Use in AI stack:
Used for Retrieval-Augmented Generation (RAG) — the agent retrieves relevant chunks from Pinecone to give context to the LLM.

#### 🔁 Alternatives:

- 🧬 Qdrant – open-source, production-ready vector DB with REST/gRPC APIs.
- 💎 Weaviate – semantic graph + vector search, supports hybrid queries.
- ⚡ Milvus – high-performance open-source vector DB, supports huge datasets.
- 🪣 Chroma – lightweight, embedded vector store (good for local dev).
- 📚 Redis Vector / PostgreSQL pgvector – add-on vector search inside existing databases.

## ✅ In one line (with flexibility):

n8n (or Airflow) automates → LangChain (or LlamaIndex) orchestrates → Ollama (or vLLM) thinks → Pinecone (or Qdrant) remembers.