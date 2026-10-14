# Mohammed Rafay

**Founder, [MemorySync](https://memorysync.io)** · Memory infrastructure for autonomous systems

Agents don't fail because models are weak. They fail because state is mismanaged: context gets stuffed, truncated, or forgotten. I build the layer that fixes that.

---

## Focus & Core Architecture

**The problem:** every agent hits the same walls. Context windows are finite, token costs compound with every turn, and naive "stuff the history into the prompt" approaches turn long-running agents into slow, expensive, forgetful ones.

**What I work on:**

- **Long-term context retention.** Persisting what an agent has learned across sessions, tools, and runs, so state survives the context window instead of being limited by it.
- **Memory graphs.** Modeling memory as connected entities and relationships rather than a flat pile of embeddings, so retrieval follows meaning and not just similarity.
- **Adaptive retrieval.** Pulling the smallest useful slice of memory for the task at hand, ranked and shaped per request, instead of dumping everything that loosely matches.
- **Token bloat control.** Treating tokens as a budget. Compaction, deduplication, and selective recall keep prompts lean without discarding signal.
- **Hot / warm / cold tiering.** Active working memory stays fast and close, recent context sits one hop away, and long-tail history is stored cheaply and recalled on demand. Memory moves between tiers based on how it is actually used.

---

## Active Projects

### [MemorySync](https://memorysync.io)

Production memory infrastructure for AI agents: long-term retention, graph-structured memory, and adaptive retrieval behind a simple API.

**How it's split:**

- **Core engine runtime: managed service.** The memory engine (storage, tiering, graph construction, retrieval) runs as a hosted service, so teams get production-grade memory without operating it themselves.
- **Framework adapters: fully open-source.** Every client layer and plugin below is open for the developer community to read, fork, and extend.

**Native integrations**

Claude Code · Cursor · n8n · Dify · Pipecat · LangGraph · Agno · Mastra · Vercel AI SDK · CrewAI

Each adapter is built to fit the idioms of its framework: the same persistent memory underneath, wired in the way that ecosystem expects. Repos live under [@memorysyncio](https://github.com/memorysyncio).

---

## Core Tooling Systems

I work close to the runtime: vector index runtimes that serve low-latency recall, async streaming pipelines that keep memory writes off the agent's hot path, and containerized server architectures that make the whole system deployable and reproducible.

---

**Building in public:** [memorysync.io](https://memorysync.io) · [@memorysyncio](https://github.com/memorysyncio)
