# MCPFusion Developer Prover MCP Server

LLMs have never been trained on MCPFusion. They use raw z.object(), skip Presenters, mix semantic verbs, and violate MVA layering. This tool teaches the framework through structured reflection — forcing the agent to prove it understands defineModel(), Presenters, and the Model-View-Ag...

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mcpfusion-developer-prover)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
LLMs don't know MCPFusion. They weren't trained on it. They fall back to what they know: raw Zod schemas, manual success() wrapping, inline JSON responses, and flat file structures. The result: MCP servers that work but violate every MVA principle.

### The Problem

- **Raw z.object()** — Bypasses defineModel(), losing hidden field stripping, fillable profiles, timestamps, and .toApi() alias resolution
- **Missing Presenters** — Handlers dump raw JSON, losing egress validation, JIT rules, server-rendered UI, agentLimit, and action suggestions
- **Wrong semantic verbs** — f.mutation() for reads, f.query() for writes — misleading the LLM about side effects
- **Manual success()** — Wrapping data manually when .handle() does it automatically
- **Inline schemas** — z.object() in tool files instead of Models in models/ layer

### How It Works

5 Decision Pivots teach and validate MCPFusion mastery:

1. **mvaRespected** — Model→Presenter→Tool layering, downward imports only
2. **modelUsed** — defineModel() for every entity with m.casts(), m.hidden(), m.fillable()
3. **presenterAttached** — .returns(Presenter) on every data-returning tool
4. **semanticVerbCorrect** — f.query()=read, f.mutation()=write, f.action()=neutral
5. **fileStructureCorrect** — models/, views/, agents/ separation


## Available Tools
- **validate_mcpfusion_implementation**: MVA is a CONCEPTUAL separation of responsibilities, NOT a folder naming convention. Before writing or validating MCPFusion code, call this tool to PROVE architectural compliance. Key rules: (1) EVERY entity uses defineModel() with m.casts() — NEVER raw z.object(). defineModel() provides m.hidden(), m.fillable(), m.timestamps(), m.guarded(), .toApi(). z.object() loses all of these, (2) EVERY tool that returns data uses .returns(Presenter). The Presenter validates, strips hidden fields, injects rules, renders UI. createPresenter().schema(Model) or definePresenter({ schema: Model }), (3) SEMANTIC VERBS: f.query() for reads (readOnly, cacheable, safe to retry). f.mutation() for writes (destructive, requires confirmation). f.action() for neutral operations (calculations, validations), (4) TOOL INPUT uses .withString()/.withNumber()/.withBoolean()/.withEnum() — NOT z.object(). For many params: .withStrings({...}), .withOptionalStrings({...}). For model-driven input: .fromModel(Model, "create"), (5) .handle() auto-wraps data with success() — NEVER call success() manually, (6) RESPONSIBILITY SEPARATION: Model, View, and Agent logic in separate modules — not mixed in one file. Additional layers (e.g. engine/ for pure business logic) are perfectly valid, (7) .instructions() on every tool for AI-First guidance, (8) f.error() for self-healing errors with .suggest(), .actions(), .retryAfter(). If rejected, fix the MCPFusion pattern violation.

Structured reflection tool for MCPFusion framework development — forces MVA (Model-View-Agent) conceptual compliance: defineModel() enforcement, Presenter attachment, semantic verb correctness. LLMs have never been trained on MCPFusion — they default to raw z.object(), skip Presenters, mix semantic verbs, and violate MVA responsibility separation. This tool teaches the framework through structured reflection. Catches MVA Violated (Model, View, and Agent responsibilities mixed in one module — MVA enforces conceptual separation: Models define data shapes, Presenters handle egress, Tools expose to LLMs. Mixing defineModel() and .handle() in one file breaks this contract), Raw Schema Detected (using z.object() instead of defineModel() for entity schemas — const UserSchema = z.object({ name: z.string(), email: z.string() }) loses every MCPFusion feature: no m.hidden() for sensitive fields (password hashes, API keys), no m.fillable() profiles for create vs. update contexts, no m.timestamps() for automatic created_at/updated_at, no m.guarded() for mass-assignment protection, no .toApi() for alias resolution. defineModel(User).casts(m => ({ name: m.string(Name), email: m.string(Email) })) provides all of these. z.object() is Zod — defineModel() is MCPFusion), Presenter Missing (returning raw data from .handle() without .returns(Presenter) — a tool that returns { users: [...] } without a Presenter sends raw database objects to the client. Hidden fields (password_hash, internal_id) leak. No UI rendering (echarts, mermaid, summary). No agent suggestions (suggestActions for next steps). No collection limiting (agentLimit). createPresenter().schema(UserModel) or definePresenter({ schema: UserModel }) — the Presenter IS the egress gate), and Semantic Verb Wrong (using f.action() for a read-only query or f.query() for a destructive write — f.query() marks the tool as readOnly — it can be safely cached, parallelized, and retried. f.mutation() marks the tool as destructive — agents must confirm before execution, responses are never cached. Using f.action() for everything wastes these semantic guarantees. GET /users is f.query(). POST /users is f.mutation(). A calculator is f.action()). NOTE: MVA is a CONCEPTUAL separation of responsibilities, NOT a folder naming convention. Implementations may organize files however they want (including additional layers like engine/ for pure business logic) as long as Model, View, and Agent responsibilities remain separated. Call once per tool or feature being implemented


## Installation & Usage

To install and use the **MCPFusion Developer Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mcpfusion-developer-prover](https://vinkius.com/mcp/mcpfusion-developer-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
