# Unified AI Workspace (name TBD)

A self-hosted, cost-first AI workspace. Plug in any model with your own API keys, switch models mid-chat without losing context, and extend capabilities via tools (MCP, plugins).

## ✨ Why
Developers need accurate, explainable, and low-cost AI. Existing UIs (LibreChat, Open WebUI, AnythingLLM, Lobe Chat, etc.) cover some of this space, but we unify **multi-model access, shared context, cost-aware routing, and tool integration** in one private, extensible UI.

## 🚀 Features (MVP → Future)
- Multi-model chat with **mid-chat switching**  
- Shared **context pack** (session memory + summaries)  
- **Cost meter & budget router** (optimize spend, avoid surprises)  
- **Local-first fallback** (Ollama or LM Studio)  
- **MCP support & plugin SDK** (extend with tools)  
- **Explainability panel** (prompt + context trace)  
- Desktop packaging (Tauri) + self-host (Docker)  

## 🛠️ Quick start
```bash
git clone https://github.com/<your-org>/<your-repo>.git
cd unified-ai
pnpm install
pnpm dev
```
