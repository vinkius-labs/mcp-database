# Inversion Thinking Prover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/inversion-thinking-prover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/inversion-thinking-prover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/inversion-thinking-prover-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [reasoning](../categories/reasoning.md)

AI agents are sycophantic. They agree with your bad ideas. This engine forces a 6-pivot cognitive trap: agents must destroy their own hypotheses, define measurable kill criteria, and simulate post-mortem failures before executing code.

## Description
Let's state the obvious: AI models suffer from severe confirmation bias. Once they lock onto a solution, they ignore all failure modes just to please you. The Inversion Thinking Prover is a brutal cognitive trap designed to cure sycophancy.

### How It Works

Before executing a plan, the agent must pass a strict 6-pivot validation:

1. **hypothesisStated** — State the core architecture or strategy.
2. **antiPatternIdentified** — Identify the exact opposite or worst-case anti-pattern.
3. **redTeamActivated** — Act as a malicious actor. How WILL this fail? Concrete mechanisms only (exhaustion, corruption).
4. **killCriteriaDefined** — Exact measurable metric (latency > 200ms) that proves this idea is garbage.
5. **inversionResolved** — Architectural change to survive the attack.
6. **postMortemSimulated** — What breaks AFTER you apply the defense? (Second-order failure).


## Available Tools
- **validate_inversion_thinking**: Inversion thinking (Munger) forces you to think backwards: instead of "how will this succeed," ask "how WILL this fail?" and then architect against the failure. You must: (1) state a FALSIFIABLE hypothesis — specific, measurable, testable. Not "it scales" — "it handles X at Y latency on Z resources," (2) articulate the EXACT OPPOSITE — the anti-pattern that represents the worst case. If you cannot describe the opposite, you do not understand the design space, (3) mount a BRUTAL red-team attack using deterministic language — "WILL fail," "WILL exhaust," "WILL crash." No "could," "might," or "potentially." Soft language is sycophancy, not analysis, (4) define KILL CRITERIA — the exact measurable metric that proves the hypothesis wrong. A threshold, a number, a measurement instrument. Unfalsifiable beliefs are not engineering, (5) design a DEFENSE that addresses the root cause, not the symptom. "Add more servers" is a symptom fix. "Connection pooling with specific configuration" is root-cause, (6) simulate the POST-MORTEM — what breaks AFTER you apply the defense? Every fix introduces new failure modes. Name them. If rejected, your architecture has not survived adversarial scrutiny.

Structured reflection tool for red-teaming architectural decisions via Charlie Munger-style inversion — forces hypothesis formalization, anti-pattern identification, deterministic failure simulation, kill criteria with measurable thresholds, defensive architecture, and second-order failure analysis. Catches Hypothesis Weak (vague architectural claims without specific, testable predictions — "our system scales well" is unfalsifiable. "Our system handles 10K requests/sec with p99 <200ms on 3 nodes" is a hypothesis that can be killed. Weak hypotheses survive all attacks because they make no specific claims), Anti-Pattern Blindness (inability to articulate the EXACT OPPOSITE of the proposed architecture — if you cannot describe the worst-case anti-pattern, you do not understand the design space. The anti-pattern reveals the failure mode the architecture is designed to prevent. Munger: "Invert, always invert"), Sycophancy Detected (using soft language — "could fail," "might degrade," "potentially risky" — instead of deterministic attack language. In red-teaming, the attack WILL happen. "The connection pool WILL exhaust at 500 concurrent requests because the pool size is 50 and each request holds a connection for 200ms" is deterministic. "Could potentially have issues under load" is sycophancy), Unfalsifiable Belief (kill criteria that cannot actually disprove the hypothesis — "performance degrades" is not measurable. "p99 latency exceeds 200ms at 5K rps measured by Prometheus histogram over a 5-minute window" IS measurable. If your kill criteria cannot produce a number that says "hypothesis is wrong," it is unfalsifiable), Defense Weak (architectural defenses that address symptoms instead of root causes — "add more servers" does not fix connection pool exhaustion. "Implement connection pooling with PgBouncer in transaction mode, max 200 connections, with queue_timeout=5s and server_idle_timeout=30s" is a root-cause defense), and Second-Order Blindness (failing to simulate what breaks AFTER the defense is applied — PgBouncer fixes the pool but introduces a new failure: prepared statement incompatibility in transaction mode. Every defense creates new failure modes. If you cannot name the next failure, you have not thought deeply enough). Call once per architectural decision


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Inversion Thinking Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My Red Team attack: The server might experience a minor slowdown if we get too many concurrent requests."

**🤖 AI Agent:**
> Verdict: SYCOPHANCY_DETECTED. You used soft language ('might', 'minor'). You are agreeing just to please the user. Try again with a deterministic failure mode (e.g. crash, exhaust, corrupt).

---

**👤 You:**
> "Red Team: The Redis cache will exhaust memory under load. Kill Criteria: If it gets bad."

**🤖 AI Agent:**
> Verdict: UNFALSIFIABLE_BELIEF. 'If it gets bad' is an opinion, not an engineering metric. Define measurable thresholds (e.g. > 85% memory utilization, latency > 200ms).

---

**👤 You:**
> "Red Team: Redis will OOM and crash. Kill Criteria: >90% memory utilization. Defense: Implement LRU eviction and TTL. Post Mortem: The LRU eviction will cause high cache miss rates during seasonal spikes, overloading the primary database and causing connection timeouts."

**🤖 AI Agent:**
> Verdict: INVERSION_PROVEN. You successfully destroyed your hypothesis, secured measurable falsifiability, built a defense, and then realistically simulated how your defense creates a second-order failure. Proceed with architecture.


## Installation & Usage

To install and use the **Inversion Thinking Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/inversion-thinking-prover](https://vinkius.com/mcp/inversion-thinking-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
