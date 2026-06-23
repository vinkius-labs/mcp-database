# LangSmith (LLM Observability & Hub) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/langsmith-llm-observability-hub)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Monitor LLM apps via LangSmith — track traces, audit prompt templates, and manage evaluation datasets.

## Description
Connect your **LangSmith** account to any AI agent and take full control of your LLM observability, tracing, and prompt management through natural conversation.

### What you can do

- **Trace Orchestration** — List active tracing projects and retrieve detailed execution logs for specific LLM invocation runs directly from your agent
- **Performance Telemetry** — Extract precise metrics including token consumption, prompt latency, and exact error strings from your AI pipelines
- **Prompt Hub Access** — Navigate and retrieve managed prompt templates, variable definitions, and version histories hosted in the LangChain Hub
- **Evaluation Datasets** — Enumerate curated 'golden' datasets used for automated evaluation of prompt logic or few-shot injection models
- **Human-in-the-Loop Audit** — Monitor active annotation queues where human reviewers assess the alignment, accuracy, and safety of generated LLM traces
- **Agentic Step Analysis** — Deep-dive into multi-turn agentic workflows to understand nested tool calls and internal reasoning paths securely

### How it works

1. Subscribe to this server
2. Enter your LangSmith API Key and Endpoint
3. Start monitoring your LLM infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **LLM Engineers** — debug complex agentic traces and measure prompt performance through natural conversation without manual UI filtering
- **AI Developers** — retrieve the latest prompt templates from the Hub and verify evaluation dataset structures directly from your workspace
- **AI Analysts** — audit human feedback queues and report on overall model grounding and accuracy across multiple tracing projects


## Available Tools (6)
- **list_projects**: Maps out the boundaries of distinct AI pipelines currently monitored by LangSmith.

List all active LangSmith tracing projects/sessions
- **list_runs**: Isolates the raw interactions containing prompts sent to and responses received from the AI models.

List explicit LLM invocation runs within a specific project
- **get_run**: Get precise telemetry for a single LLM invocation run
- **list_datasets**: List all evaluation and fine-tuning datasets mapped in LangSmith
- **list_prompts**: Extract prompt templates hosted in the LangChain Hub
- **list_annotation_queues**: List active human-in-the-loop annotation queues


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LangSmith (LLM Observability & Hub)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active tracing projects in LangSmith"

**🤖 AI Agent:**
> I've found 4 active tracing projects: 'Production-Bot-V2', 'Staging-RAG-Explorer', 'Customer-Support-Agent', and 'Internal-Testing-Suite'. Which one would you like to see the recent runs for?

---

**👤 You:**
> "Show me the telemetry for the last run in the 'Production-Bot-V2' project"

**🤖 AI Agent:**
> Retrieving data for run ID 'run-98765'… The execution was successful. Total tokens: 1,420 (Prompt: 850, Completion: 570). Latency: 2.4s. The agent successfully used the 'Web-Search' tool before generating the answer. No errors detected.

---

**👤 You:**
> "List all prompts hosted in our Hub repository"

**🤖 AI Agent:**
> I've identified 3 prompts in your Hub: 'summarization-agent-v1', 'customer-service-v3', and 'data-extraction-helper'. I can retrieve the full instruction text and version history for any of these.


## ❓ FAQ

**Q: Can I see the token usage for a specific LLM run through my agent?**
Yes. Use the `get_run_telemetry` tool with a specific Run ID. Your agent will retrieve the exact token count (prompt + completion) and latency metrics calculated by LangSmith for that interaction.

**Q: How do I fetch a prompt template from the LangChain Hub using natural language?**
The `list_prompts` tool allows your agent to navigate your hosted Hub repository. You can ask your agent to find a specific prompt by name to inspect its instruction text, variables, and version history.

**Q: Can my agent check the status of human annotation queues?**
Absolutely. Use the `list_annotation_queues` tool to retrieve all active queues where human feedback is being collected. Your agent can report on the number of pending traces and general alignment scores established by your reviewers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/langsmith-llm-observability-hub](https://vinkius.com/mcp/langsmith-llm-observability-hub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LangSmith (LLM Observability & Hub)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `langsmith-llm-observability-hub` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LangSmith (LLM Observability & Hub)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "langsmith-llm-observability-hub": {
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
