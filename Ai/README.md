<!-- AI research home -->
# AI Research Workspace
This folder captures notes, references, and experiments across the AI stack that powers current projects.

## Quick Links
- [Components Overview](Components_Overview.md) - roles, alternatives, and decision notes for the orchestration stack (n8n, LangChain, Ollama, Spec Kit, Pinecone, etc.).
- [MCP Servers](Mcp/MCP.md) - primer on Model Context Protocol servers and how they extend agent capabilities.

## Focus Areas
- **Workflow automation** - evaluate how tools like n8n trigger pipelines, handle embeddings, and surface actions to agents.
- **Orchestration frameworks** - compare LangChain with alternatives (LlamaIndex, Semantic Kernel) for building resilient agent flows.
- **Local model hosting** - track Ollama configurations and swaps with cloud-hosted APIs when higher reasoning or scale is needed.
- **Spec-driven delivery** - document lessons learned from adopting GitHub Spec Kit to keep AI coding runs aligned with specs.
- **Context extension** - explore MCP servers and other adapters for exposing internal data, task systems, or custom tooling safely.

## How to Use This Folder
1. Start with `Components_Overview.md` to understand the high-level architecture.
2. Dive into subfolders (like `Mcp/`) for protocol-specific research.
3. Append new findings or experiments as additional Markdown files and keep link references updated here so the index stays useful.

> Tip: When adding a new technology note, include why it matters for the stack (use cases, integration points, trade-offs) to make the research actionable.
