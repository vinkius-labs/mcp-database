# New Relic AI (LLM Observability) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/new-relic-ai-llm-observability)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/new-relic-ai-llm-observability-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/new-relic-ai-llm-observability-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Monitor and audit LLM telemetry via New Relic AI — track token costs, p95 latency, and user feedback.

## Description
Connect your **New Relic AI** account to any AI agent and take full control of your LLM observability, token cost tracking, and performance analytics through natural conversation.

### What you can do

- **LLM Telemetry Audit** — Retrieve detailed LLM chat completion messages and prompt inputs directly from your agent to understand literal model behavior in real-time
- **Token Cost Tracking** — Execute structural extraction of model costs to calculate exact USD token consumption across your entire AI infrastructure securely
- **Performance Monitoring** — Extract p95 latency matrices and average response times to ensure your LLM text generation remains performant and sub-second
- **User Feedback Loop** — Retrieve chronological feedback messages and 1-5 rating scores dumped by human supervisors to identify quality regressions natively
- **Custom NRQL Execution** — Run sophisticated read-only queries using the New Relic Query Language (NRQL) to extract rich insights from multi-tenant AI datasets instantly
- **Custom Event Injection** — Post atomic generic telemetry rows to track internal agent states and custom behavioral markers across your observability pipeline
- **Resource Discovery** — Enumerate active APM apps, dashboards, and alert policies to audit your AI environment's structural health and PagerDuty configurations

### How it works

1. Subscribe to this server
2. Enter your New Relic API Key and Account ID
3. Start monitoring your AI stack from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Engineers** — monitor LLM prompt performance and verify model accuracy through natural conversation without manual dashboard navigation
- **Observability Leads** — track global AI token costs and p95 latency benchmarks directly from your workspace to optimize infrastructure spend
- **DevOps Teams** — audit APM app health and verify alert policy triggers across multiple AI environments efficiently


## Available Tools
- **list_alert_policies**: Inspect deep internal arrays mitigating specific Plan Math
- **list_apm_apps**: Dispatch an automated validation check routing explicit Gateway history
- **custom_nrql**: Note that NRQL is read-only.

Irreversibly vaporize explicit validations extracting rich Churn flags
- **list_dashboards**: Identify precise active arrays spanning native Gateway auth
- **query_llm_errors**: Identify precise active arrays spanning native Hold parsing
- **query_llm_costs**: Perform structural extraction of properties driving active Account logic
- **query_llm_events**: Identify bounded CRM records inside the Headless New Relic Platform
- **query_llm_feedback**: Retrieve explicit Cloud logging tracing explicit Vault limits
- **query_llm_latency**: Provision a highly-available JSON Payload generating hard Customer bindings
- **post_custom_event**: /events` inserting absolute generic `CustomAITelemetry` rows tracking internal agent state.

Enumerate explicitly attached structured rules exporting active Billing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **New Relic AI (LLM Observability)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the last 5 LLM events for the 'OpenAI' vendor"

**🤖 AI Agent:**
> Retrieving LLM events… I've identified 5 recent messages through the OpenAI module. Highlights: 1) Chat completion 'task-123' (Tokens: 1,500, Cost: $0.03), 2) Prompt 'User Query Alpha' (Status: Success). Would you like to see the literal prompt text for any of these?

---

**👤 You:**
> "What is my total LLM token cost for the last 24 hours?"

**🤖 AI Agent:**
> Retrieving cost metrics… Your total LLM token spend for the last 24 hours is $12.45. This is distributed across 'gpt-4o' ($8.50), 'gpt-3.5-turbo' ($2.45), and 'claude-3-sonnet' ($1.50). Spend is trending 5% lower than yesterday.

---

**👤 You:**
> "Run NRQL: SELECT count(*) FROM LlmEvent WHERE duration > 2 SINCE 1 hour ago"

**🤖 AI Agent:**
> Executing custom NRQL query… I've identified 12 LLM events in the last hour that exceeded 2 seconds in duration. This represents approximately 3% of your total traffic. Would you like me to facet these slow events by model or region?


## Installation & Usage

To install and use the **New Relic AI (LLM Observability)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/new-relic-ai-llm-observability](https://vinkius.com/mcp/new-relic-ai-llm-observability)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
