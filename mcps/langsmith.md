# LangSmith MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/langsmith)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/langsmith-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/langsmith-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Observability and evaluation platform for LLM applications — monitor traces, debug agent runs, and track performance metrics across your AI stack.

## Description
Connect your AI agent to **LangSmith** — the observability platform from the LangChain team that gives you complete visibility into your LLM applications.

### What you can do

- **List Projects** — View all tracing projects with aggregate metrics: total runs, median latency, feedback scores, and creation dates
- **List Runs** — Browse recent traces in any project. See run names, types (LLM, chain, tool), status (success/error), token usage, and timing
- **Run Details** — Deep-dive into any specific run to see its full execution trace, inputs, outputs, and associated feedback

### How it works

1. Subscribe to this server
2. Enter your LangSmith API key (5,000 free traces/month)
3. Your agent can now monitor and debug LLM applications

### Who is this for?

- **AI Engineers** — monitor LLM calls, chains, and agent actions in production
- **ML Teams** — track experiment performance, compare model outputs, and identify regressions
- **DevOps** — set up alerts for error rates, latency spikes, and cost anomalies in AI workloads


## Available Tools
- **langsmith_get_run**: Useful for debugging specific LLM calls or agent actions.

Get detailed information about a specific run/trace by its ID
- **langsmith_list_projects**: Each project groups related traces together and shows aggregate metrics like total runs, median latency, and feedback counts.

List all tracing projects in your LangSmith account with run counts, latency stats, and feedback metrics
- **langsmith_list_runs**: Each run represents a single LLM call, chain execution, or agent action. Shows status (success/error), latency, and token consumption.

List recent traces/runs in a specific LangSmith project. Shows run names, types, status, token usage, and timing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LangSmith** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my LangSmith projects and show their metrics."

**🤖 AI Agent:**
> Found 4 projects:

| Name | ID | Runs | Latency | Created |
|---|---|---|---|---|
| production-agent | `a1b2c3d4` | 12,450 | 340ms | 2026-01-15 |
| staging-chatbot | `e5f6g7h8` | 3,200 | 280ms | 2026-02-20 |
| research-rag | `i9j0k1l2` | 890 | 520ms | 2026-03-01 |
| test-evaluations | `m3n4o5p6` | 150 | 190ms | 2026-03-28 |

---

**👤 You:**
> "Show me the last 5 runs in my production-agent project."

**🤖 AI Agent:**
> Last 5 runs in 'production-agent':

| Name | ID | Type | Latency | Created |
|---|---|---|---|---|
| agent_executor (success) | `r1s2t3` | chain | 1,250 tokens | 2026-04-04 |
| gpt-4o (success) | `u4v5w6` | llm | 890 tokens | 2026-04-04 |
| tool:web_search (success) | `x7y8z9` | tool | 340ms | 2026-04-04 |
| agent_executor (error) | `a0b1c2` | chain | 450 tokens | 2026-04-03 |
| gpt-4o (success) | `d3e4f5` | llm | 1,100 tokens | 2026-04-03 |

---

**👤 You:**
> "Get details on the failed run a0b1c2."

**🤖 AI Agent:**
> Run details for `a0b1c2`:

| Name | ID | Type | Latency | Created |
|---|---|---|---|---|
| agent_executor \| chain \| error | `a0b1c2` | chain | 450 tokens | 2026-04-03 |

Error: Tool 'web_search' returned timeout after 30s. The agent retried 3 times before failing.


## Installation & Usage

To install and use the **LangSmith** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/langsmith](https://vinkius.com/mcp/langsmith)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
