# Hi, I’m **Antonio Borge Rees** 👋

### Software Engineer · Agentic Orchestration · Frontier AI Systems

I build **agent-orchestrated systems** with a strong emphasis on **absolute observability**, **SOLID design principles**, and **explicit structure**.

Rather than treating agents as scripts or demos, I focus on the *systems around them*: how they coordinate, how they reason over data, how they fail, and—most importantly—how we understand what they’re doing while they run.

I’m currently enrolled in the [**Digital Futures – Frontier AI training programme**](https://digitalfutures.com/insights/individuals/frontier-ai-launch-your-journey-to-shape-the-future-of-technology), focused on building practical, production-grade AI systems that shape the future of technology.

---

## Design Philosophy

My recent work is driven by two core beliefs:

1. **Observability is truth: if it is not observable, it didn't happen.**
2. **The harness often matters more than the model. Agents scale through context and structure.**

As systems become more autonomous, the cost of *not* understanding them increases dramatically. My projects aim to push autonomy forward **without sacrificing debuggability, reasoning, or control**.

This philosophy directly led to the creation of **Stageflow** and **Unified Content Protocol (UCP)**.

---

## Stageflow

**Observable, composable DAG orchestration for agentic pipelines (Python)**

Stageflow was born from a very practical need:

* I needed to **parallelise complex pipelines** to **reduce latency** 
* I wanted those pipelines to be **modular and reusable**
* I wanted to stop rewriting orchestration glue code
* And I needed **observability as a first-class feature**, not an afterthought

I realised that designing pipelines was not hard- it is everything else around it, from observability to guardrails to reliability measures. Stageflow treats orchestration itself as a core domain. Pipelines are explicit DAGs, stages have clear contracts, and execution is observable by default.

**Key ideas**

* Stages execute as soon as dependencies resolve → maximum parallelism
* Pipelines are defined fluently and composed safely
* Cross-cutting concerns live in interceptors, not business logic
* Events, correlation IDs, and structured logging are built in
* Async-first execution using `asyncio`
* Zero external dependencies in the core library

**Stage kinds**
`TRANSFORM · ENRICH · ROUTE · GUARD · WORK · AGENT`

This makes Stageflow especially well-suited for:

* Multi-step LLM and agent pipelines
* Guardrailed, observable AI workflows
* Long-running automation where failures must be understood, not hidden

Stageflow is designed for environments where things *will* fail — and where understanding **what happened, where, and why** matters more than raw throughput.

[**See how it works**](stageflow-landing-page.netlify.app)

**Try it out:** `pip install stageflow-core`

**Repo:** [https://github.com/Antonio7098/stageflow](https://github.com/Antonio7098/stageflow)

---

## Unified Content Protocol (UCP / UCM)

**Graph-native, agent-first representation for structured content**

Unified Content Protocol (UCP) addresses a different but complementary problem:

> *From an agent’s perspective, every data source should look the same.*

Markdown documents, JSON files, databases, HTML pages, code, tables — today, each requires bespoke handling. UCP provides a **single, unified, graph-based interface** for agents to interact with content regardless of origin.

### Graph-Native by Design

At its core, UCP (via **UCM – Unified Content Model**) is **graph-native**:

* Content is represented as nodes (blocks) with explicit edges
* Blocks are content-addressed and deterministic
* Relationships are first-class, not inferred from text
* Traversal is cheap, explicit, and predictable

This makes UCP **naturally optimised for graph traversal by LLMs and agents**. Instead of flattening documents into token-heavy text blobs, agents can walk the graph, follow semantic edges, and operate on structure directly.

### Why This Matters for LLMs

UCP is designed to be:

* **Token-efficient** — structure is encoded once, not repeated
* **Deterministic** — identical content always hashes to the same ID
* **Machine-readable** — structure is explicit, not implied
* **Safe to transform** — edits occur through validated graph operations

To an agent, the following all share the same interface:

* A Markdown document
* A JSON dataset
* A database record
* An HTML page

This enables:

* Structural reasoning instead of text-only heuristics
* Safer autonomous edits
* Reproducible transformations
* Better long-context efficiency

UCP pairs naturally with **Stageflow**, where agents operate inside observable pipelines and reason over graph-structured content.

[**See how it works**](https://ucp-landing-page.netlify.app/)

**Try it out:** `pip install ucp-content`

**Repo:** [https://github.com/Antonio7098/unified-content-protocol](https://github.com/Antonio7098/unified-content-protocol)

---

## 24-Hour Testers

**Autonomous reliability loop for continuous system testing**

24-Hour Testers operationalises agentic systems in the real world.

You describe a **System Under Test (SUT)** once, provide a canonical checklist, and agents continuously:

* Execute tests and experiments
* Write structured findings
* Generate reports
* Synthesize new backlog automatically (in infinite mode)

No babysitting. No manual triggering. Just a loop that keeps running.

This project focuses on:

* Long-running autonomy
* Observable execution
* Persistent state and resumability
* Practical reliability engineering using agents

**Repo:** [https://github.com/Antonio7098/24-hour-testers](https://github.com/Antonio7098/24-hour-testers)

---

## Learning Sprints

**Agent-guided framework for deep technical learning**

Learning Sprints formalises how an AI agent should act as a **mentor**, not a tutorial.

It provides structured workflows for:

* Defining learning goals
* Creating investigative sprints
* Walking through implementation
* Marking code and reasoning
* Adapting questions based on performance

The emphasis is on **deep understanding**, progressive synthesis, and professional habits — not surface-level completion.

**Repo:** [https://github.com/Antonio7098/learning-sprints](https://github.com/Antonio7098/learning-sprints)

---

## How These Pieces Fit Together

All of my recent work shares a common direction:

* **Stageflow** → observable orchestration of agent behaviour
* **UCP / UCM** → unified, graph-native interface for agent data
* **24h Testers** → long-running autonomous loops in practice
* **Learning Sprints** → structured agent-guided cognition

The goal is not “more agents”, but **better systems around agents** — systems that scale in autonomy *without collapsing into opacity*.

---

## 📫 Connect

[LinkedIn](https://linkedin.com/in/antonio-borge-rees-298631189) | [antoniorees74@gmail.com](mailto:antoniorees74@gmail.com)
