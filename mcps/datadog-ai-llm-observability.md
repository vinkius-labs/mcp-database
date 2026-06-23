# Datadog AI (LLM Observability) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/datadog-ai-llm-observability)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Monitor LLM performance via Datadog — track token usage, audit prompts, and monitor AI model metrics directly from any AI agent.

## Description
Connect your **Datadog** account to any AI agent and take full control of your LLM observability and AI performance monitoring through natural conversation.

### What you can do

- **LLM Metrics Auditing** — Query high-precision numeric telemetry targeting LLM Observability timeseries like token counts and latency
- **Prompt & Span Search** — Retrieve explicit APM payload contents capturing literal prompt logic and response traces limitlessly
- **AI Monitor Management** — List and create monitors to track when AI responses drop below SLI thresholds or plateau on requests
- **Dashboard Insights** — Enumerate widgets graphing global AI expenses across providers like OpenAI or Anthropic
- **Incident Tracking** — Monitor active outages and service disruptions blocking multi-agent orchestration dynamically
- **Timeline Events** — Pull pure textual deployment marks identifying exactly when dynamic LLM models were switched

### How it works

1. Subscribe to this server
2. Enter your Datadog API Key, APP Key, and Site
3. Start monitoring your AI infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Engineers** — monitor LLM latencies and token costs in real-time without leaving the dev environment
- **MLOps Teams** — audit prompt logs and trace AI model performance across different versions
- **SREs** — set up monitors for AI services and track incidents affecting agentic workflows
- **FinOps** — analyze dashboards graphing global AI infrastructure expenses and usage patterns


## Available Tools (10)
- **create_event**: Inspect deep internal arrays mitigating specific Plan Math
- **create_monitor**: Irreversibly vaporize explicit validations extracting rich Churn flags
- **list_dashboards**: Enumerate explicitly attached structured rules exporting active Billing
- **list_events**: 0 deployed".

Identify precise active arrays spanning native Gateway auth
- **list_incidents**: Dispatch an automated validation check routing explicit Gateway history
- **search_llm_spans**: Provision a highly-available JSON Payload generating hard Customer bindings
- **list_ai_monitors**: Retrieve explicit Cloud logging tracing explicit Vault limits
- **query_metrics**: g `datadog.llm_observability.tokens`.

Identify bounded CRM records inside the Headless Datadog Platform
- **submit_series**: Perform structural extraction of properties driving active Account logic
- **list_service_accounts**: Identify precise active arrays spanning native Hold parsing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Datadog AI (LLM Observability)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the average token usage for GPT-4 over the last hour"

**🤖 AI Agent:**
> Querying Datadog metrics... Average token usage for GPT-4 is 150 per request. Usage peaked at 10:30 AM with 450 tokens. Latency is within normal bounds (avg 850ms).

---

**👤 You:**
> "Search for LLM logs containing 'out of bounds error'"

**🤖 AI Agent:**
> I found 3 spans matching 'out of bounds error' in your logs. They were triggered by the 'Data-Analyzer' agent. I can provide the full prompt and stack trace for these errors.

---

**👤 You:**
> "List all active AI monitors"

**🤖 AI Agent:**
> You have 4 active AI monitors. [LLM-Latency-High] is currently in 'Alert' state, while [Token-Quota-Reached], [GPU-Utilization], and [Model-Drift] are 'OK'.


## ❓ FAQ

**Q: Can my agent check token usage for a specific LLM model?**
Yes. Use the 'query_metrics' tool with a query like 'avg:datadog.llm_observability.tokens{model:gpt-4}'. The agent will retrieve the numeric timeseries data directly from Datadog's metrics engine.

**Q: How do I search for specific prompt text in my logs?**
Use the 'search_llm_spans' tool. Provide a search query matching your prompt identifiers. The agent will pull the explicit REST maps capturing the literal prompt logic text from your Datadog logs.

**Q: Can I see if there are any active incidents affecting my AI services?**
Absolutely. The 'list_incidents' tool tracks outages and service disruptions in real-time. This allows your agent to identify exactly which external factors might be blocking your multi-agent orchestration pipelines.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datadog-ai-llm-observability](https://vinkius.com/mcp/datadog-ai-llm-observability)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Datadog AI (LLM Observability)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `datadog-ai-llm-observability` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Datadog AI (LLM Observability)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "datadog-ai-llm-observability": {
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
