# LangSmith MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/langsmith)
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


## ❓ FAQ

**Q: What is LangSmith and why do I need it?**
LangSmith is the 'Datadog for LLM applications'. Without observability, AI agents in production are black boxes — you can't see what they're doing, why they fail, or how much they cost. LangSmith traces every LLM call, chain execution, and tool use, giving you complete visibility into inputs, outputs, latency, token usage, and error rates.

**Q: Does LangSmith work only with LangChain?**
No! While LangSmith is built by the LangChain team and has native LangChain/LangGraph integration, it works with any LLM application. You can trace OpenAI, Anthropic, or any LLM provider directly using the REST API. It also integrates with CrewAI, AutoGen, and other frameworks.

**Q: How much does LangSmith cost?**
LangSmith offers a generous free tier with 5,000 traces per month — no credit card required. The Developer plan is $39/month with 50,000 traces. Enterprise plans include SSO, RBAC, dedicated support, and unlimited traces with volume discounts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/langsmith](https://vinkius.com/mcp/langsmith)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LangSmith** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `langsmith` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LangSmith** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "langsmith": {
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
