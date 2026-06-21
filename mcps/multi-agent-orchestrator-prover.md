# Multi-Agent Orchestrator Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/multi-agent-orchestrator-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

An AI designed a multi-agent system where agents 'work together seamlessly,' data 'flows naturally between them,' and failures 'self-heal.' Three days later, Agent B crashed and the pipeline froze for 14 hours — no one knew because there was no tracing. That is not orchestration — that is hope with a tech stack. This tool forces five orchestration axes: role boundaries, handoff protocols, failure containment, consensus mechanisms, and distributed tracing.

## Description
## The Problem

Ask an LLM to design a multi-agent system. It will create agents with overlapping roles because 'they're flexible.' It will skip handoff protocols because agents 'communicate naturally.' It will ignore failure isolation because the system is 'fault tolerant by design.' And it will deploy without tracing because 'we can check the logs.'

Every LLM commits five orchestration failures:
1. **Undefined Roles** — agents with overlapping responsibilities duplicate work or drop tasks. 'General purpose agent' means undefined boundary.
2. **Missing Handoffs** — data lost between transitions. No trigger conditions, no typed contracts, no failure behavior.
3. **Cascading Failures** — one agent crashes, the entire pipeline freezes. No timeouts, no retries, no circuit breakers.
4. **Absent Consensus** — two agents produce conflicting outputs. No detection, no resolution protocol, no tie-breaking.
5. **Blind Observability** — debugging is impossible. No correlation IDs, no per-agent metrics, no distributed tracing.

## How It Works

The Multi-Agent Orchestrator Prover forces the LLM to fill 5 reflection fields and commit to 5 Decision Pivots before concluding any agent architecture is production-ready.

### The 5 Orchestration Axes

| Axis | Pivot | Rule |
|---|---|---|
| **Roles** | Defined | Explicit boundary with input/output contracts and exclusions. |
| **Handoffs** | Specified | Trigger condition, typed data contract, failure behavior. |
| **Failures** | Contained | Timeout, retry with backoff, fallback, circuit breaker. |
| **Consensus** | Deterministic | Conflict detection, resolution protocol, tie-breaking rule. |
| **Observability** | Enforced | Correlation IDs, per-agent spans, metrics, alerting. |

### The Verdict Matrix

```
Axis 1 fails → ROLES_UNDEFINED
Axis 2 fails → HANDOFFS_MISSING
Axis 3 fails → FAILURES_CASCADING
Axis 4 fails → CONSENSUS_ABSENT
Axis 5 fails → OBSERVABILITY_BLIND
All pass     → ORCHESTRATION_PROVEN
```

## Why It Works

Tool calls are obligations. The LLM cannot skip role boundaries or ignore failure containment. It must define each agent's responsibility with contracts, specify handoff triggers with typed data, implement circuit breakers with thresholds, define consensus with tie-breaking rules, and enforce tracing with correlation IDs. Every rejection names the exact orchestration axis that failed.


## Available Tools
- **validate_multi_agent_orchestration**: You must: (1) define ROLES — each agent has a name, typed input/output contracts, responsibility boundary, and explicit exclusions. "General purpose" is not a role, (2) specify HANDOFFS — each agent-to-agent transition has trigger conditions, typed data contracts, and explicit failure behavior. "Passes data" is not a protocol, (3) contain FAILURES — each agent has timeout, retry policy (count + backoff), fallback, and circuit breaker. Pipeline has cascade protection. "Retry and it works" is not containment, (4) define CONSENSUS — when agents conflict, specify detection method, resolution protocol (voting, scoring, supervisor), and deterministic tie-breaking. "They agree" is hope, not architecture, (5) enforce OBSERVABILITY — correlation IDs per request, spans per agent action, per-agent metrics (latency, tokens, errors), dashboards, and alerting. "Check the logs" is not observability. If rejected, fix the specific orchestration flaw before deploying.

Structured reflection tool for multi-agent system design — forces explicit role boundaries, typed handoff protocols, per-agent failure containment, deterministic consensus mechanisms, and distributed observability before deploying any agent pipeline or agentic workflow. Catches Roles Undefined (agents with overlapping or vague responsibilities — a 4-agent pipeline where both the ResearchAgent and AnalysisAgent "summarize relevant information." Result: both agents produce summaries, the WriterAgent receives two partially overlapping inputs, the final response contains contradictions (ResearchAgent found 12 sources, AnalysisAgent found 8, 5 overlapped, 3 conflicted). 23% of pipeline outputs contained factual inconsistencies traceable to role overlap. Each agent must have: a name, explicit input/output contracts with typed fields, responsibility boundaries, and exclusion clauses — "does NOT evaluate quality" is as important as "DOES generate responses"), Handoffs Missing (agent-to-agent transitions that lose data or have no failure behavior — ResearchAgent returns confidence: 0.3 on a query. No handoff rule exists for low confidence. WriterAgent receives the low-confidence research and generates an authoritative-sounding response based on unreliable data. The user sees a fluent answer with no indication that the underlying evidence was weak. A handoff protocol must specify: trigger conditions (confidence > 0.7 AND sources >= 2), typed data contracts (what fields transfer), and failure behavior (retry with expanded query, escalate to human, return partial results with confidence warning)), Failures Cascading (one agent failure kills the entire pipeline — a 5-agent pipeline with no circuit breakers. The ExternalAPIAgent calls a rate-limited API. At 3 AM, the API returns 429 Too Many Requests. The agent retries infinitely. The pipeline hangs. 847 requests queue behind it. By 6 AM, the orchestrator OOM-kills. Every agent needs: timeout (hard limit), retry policy (count + backoff), fallback (cached results, degraded response), and circuit breaker (open after N consecutive failures). The pipeline needs: cascade protection — if >1 agent circuit is open, return graceful degradation), Consensus Absent (multiple agents produce conflicting outputs with no resolution mechanism — a fact-checking pipeline: VerifierAgent says "claim is true (confidence: 0.72)." CounterResearchAgent says "claim is false (confidence: 0.68)." No resolution protocol exists. The system returns... both? Neither? The first one? Random? Consensus requires: conflict detection (semantic similarity threshold), resolution protocol (voting, weighted scoring, supervisor arbitration), and deterministic tie-breaking (prefer higher confidence, more citations, or escalate to human)), and Observability Blind (agents operating as black boxes — "check the logs" is not observability. A 6-agent pipeline processes a request in 12 seconds. Which agent took 10 of those seconds? Which agent used 90% of the token budget? Which agent produced the error that was masked by a downstream retry? Without correlation IDs propagated across all agents, per-agent spans with latency/token metrics, per-agent error rates, and alerting thresholds — every production issue is a forensic investigation). Call once per agent architecture or pipeline before deployment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Multi-Agent Orchestrator Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a research agent and a writer agent. The research agent finds information and the writer agent writes the response. They work together seamlessly and communicate naturally."

**🤖 AI Agent:**
> HANDOFFS_MISSING — 'Seamlessly' is hope, not architecture. When does the research agent pass to the writer? What trigger condition — confidence threshold, source count, timeout? What data shape does the writer expect — { sources: Source[], summary: string, confidence: number }? What if research finds nothing — does the writer wait forever? Define trigger conditions, typed data contracts, and failure behavior for each transition.

---

**👤 You:**
> "ResearchAgent: finds docs, boundary: does NOT write responses. Input: { query: string }. Output: { sources: Source[], confidence: number }. Handoff: triggers when confidence > 0.7 AND sources >= 2, else retries with expanded query. WriterAgent: generates response from research. Timeout: 30s research, 60s writer. Retry: 2x with backoff. Fallback: cached results. Circuit breaker: 3 failures → open. Consensus: supervisor scores by evidence-coverage. Tracing: UUID correlation, per-agent spans, Prometheus metrics, error_rate > 5% → alert."

**🤖 AI Agent:**
> ORCHESTRATION_PROVEN — Multi-agent orchestration validated. Roles: explicit boundaries with typed contracts and exclusions. Handoffs: trigger condition (confidence > 0.7, sources >= 2) with retry fallback. Failures: timeouts, retries with backoff, cached fallback, circuit breaker at 3 failures. Consensus: supervisor agent scores by evidence-coverage. Observability: UUID correlation, per-agent spans, Prometheus metrics with 5% error alerting. Production-ready agent architecture.

---

**👤 You:**
> "Our agents have clear roles and handoff protocols. If an agent fails, the system auto-recovers — it's fault tolerant by design. We added logging so we can debug issues when they come up."

**🤖 AI Agent:**
> FAILURES_CASCADING — 'Fault tolerant by design' and 'auto-recovers' are claims, not strategies. What is the timeout per agent? What is the retry policy — how many retries, with what backoff? What is the fallback if the agent is permanently down? What is the circuit breaker threshold? Also: 'logging for debugging' is not observability — implement correlation IDs, per-agent metrics, and automated alerting.


## ❓ FAQ

**Q: Do I need this with only two agents?**
Yes. Two agents still need role boundaries, a handoff protocol, failure containment, and observability. The failure modes don't care about agent count — they care about architectural discipline. A 2-agent system with undefined handoffs fails the same way a 20-agent system does.

**Q: What is a consensus mechanism for agents?**
When two agents produce conflicting outputs, a consensus mechanism resolves the conflict deterministically. Options: confidence scoring (highest confidence wins), supervisor agent review, voting with tie-breaking rules, evidence-coverage scoring. 'They usually agree' is not a mechanism — it is hope that collapses the first time agents disagree.

**Q: Does it generate agent architectures?**
No. It computes nothing. It validates that your agent architecture passes five structural checks — role boundaries, handoff protocols, failure containment, consensus, and observability. The design is yours. The discipline is enforced by the tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/multi-agent-orchestrator-prover](https://vinkius.com/mcp/multi-agent-orchestrator-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Multi-Agent Orchestrator Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `multi-agent-orchestrator-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Multi-Agent Orchestrator Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "multi-agent-orchestrator-prover": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
