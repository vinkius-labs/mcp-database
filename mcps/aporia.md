# Aporia MCP Server

Monitor AI models and validate LLM interactions with guardrails directly from your AI agent to ensure safety and observability.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/aporia)

## Overview
**Category:** fort-knox
**Tools Count:** 7

## Description
Connect your **Aporia** workspace to any AI agent to enforce strict guardrails, monitor ML model performance in real time, and audit custom dashboards directly through natural conversation.

### What you can do

- **Guardrail Validation** — Instantly validate LLM messages against your configured Aporia guardrails to detect toxicity, PII, and off-topic responses
- **Model Observability** — List instrumented machine learning and LLM models, and fetch their architectural details
- **Performance Metrics** — Retrieve real-time metrics highlighting operational performance and potential data drift
- **Active Monitors** — View and trigger active monitors to immediately check for data integrity issues or performance degradation
- **Dashboards** — Access custom dashboards that aggregate your critical observability metrics

### How it works

1. Subscribe to this server
2. Enter your Aporia API Key
3. Protect your prompt chains and manage your AI infrastructure directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI engineers** — enforce guardrails over inputs and outputs during development without swapping contexts
- **Data scientists** — track model drift and analyze production metrics instantly
- **MLOps teams** — trigger monitors on demand and visualize custom observability dashboards from a single chat pane
- **Risk officers** — guarantee compliance checking against PII and hateful content dynamically


## Available Tools
- **list_models**: List Aporia monitored machine learning and LLM models
- **get_model**: Get specific details for a monitored Aporia model
- **list_monitors**: List configured Aporia monitors for a specific model
- **trigger_monitor**: Trigger an immediate run of a specific Aporia monitor
- **validate_guardrails**: g. toxicity, PII, off-topic). Pass an array of messages.

Validate LLM interactions against Aporia guardrails
- **list_dashboards**: List custom dashboards configured in the Aporia workspace
- **get_metrics**: Get performance and drift metrics for an Aporia monitored model


## Installation & Usage

To install and use the **Aporia** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aporia](https://vinkius.com/mcp/aporia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
