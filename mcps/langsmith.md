# LangSmith MCP Server

Observability and evaluation platform for LLM applications — monitor traces, debug agent runs, and track performance metrics across your AI stack.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/langsmith)

## Overview
**Category:** friends-mcp
**Tools Count:** 3

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


## Installation & Usage

To install and use the **LangSmith** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/langsmith](https://vinkius.com/mcp/langsmith)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
