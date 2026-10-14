<h1 align="center">MOHAMMED RAFAY</h1>

<p align="center">
  🧠 <b>Founder, <a href="https://memorysync.io">MemorySync</a></b> · Memory infrastructure for autonomous systems
</p>

<p align="center">
  Agents don't fail because the model is weak. They fail because their state is mismanaged. I build the layer that fixes that.
</p>

## ⚙️ Focus & Core Architecture

Context windows are finite and tokens are a budget. I work on keeping long-running agents fast, cheap, and coherent:

- 🗄️ **Long-term retention** that outlives the context window and carries across sessions and tools
- 🕸️ **Memory graphs** that retrieve by relationship and meaning, not just vector similarity
- 🎯 **Adaptive retrieval** that returns the smallest useful slice instead of everything that loosely matches
- 🔥 **Hot / warm / cold tiering** that moves memory between tiers based on how it is actually used, so token bloat stays under control

## 🚀 Active Projects

**[MemorySync](https://memorysync.io)** is production memory infrastructure for AI agents.

- 🔒 **Core engine:** a managed service
- 🔌 **Framework adapters:** fully open-source at [@memorysyncio](https://github.com/memorysyncio), with native support for Claude Code, Cursor, n8n, Dify, Pipecat, LangGraph, Agno, Mastra, Vercel AI SDK, and CrewAI

## 🛠️ Core Tooling Systems

Vector index runtimes for low-latency recall, async streaming pipelines that keep memory writes off the agent's hot path, and containerized server architectures built for reproducible deployment.
