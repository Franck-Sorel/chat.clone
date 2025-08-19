# Architecture Overview

## Core components
- **Frontend (Next.js/Tauri)**: Chat UI, settings, plugin interface
- **API Service**: 
  - Session + context service
  - Cost meter & router
  - MCP client + plugin runtime
- **Gateway (optional)**: LiteLLM Proxy for unified providers + budgets
- **Storage**: SQLite (sessions), Vector DB (Qdrant/SQLite-vec)
- **Models**: 
  - Remote (OpenAI, Claude, Gemini, etc. via OpenRouter)
  - Local (Ollama, LM Studio)

## Context Pack
A portable JSON bundle that contains:
- Session history
- Summaries
- Retrieved knowledge snippets
- State for reproduction

## Routing
- Policy-based (budget caps, fallback)
- Token estimator before send
- Local/remote tradeoffs
