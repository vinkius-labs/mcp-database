# Arize AI MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arize-ai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/arize-ai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/arize-ai-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Automate LLM and ML observability via Arize — monitor models, track telemetry, run evaluations, and analyze data drift directly from any AI agent.

## Description
Connect your **Arize AI** observability platform to any AI agent and take full control of your Machine Learning and LLM telemetry workflows through natural conversation.

### What you can do

- **Model Monitoring & Metrics** — List all tracked ML models, extract deep configuration schemas, and fetch real-time metrics (performance, data quality, and prediction drift)
- **Evaluation & Alignment** — Launch and list automated LLM evaluation runs (e.g., Toxicity, Hallucination, PII filtering) against static datasets and ground truth baselines
- **Telemetry Ingestion** — Push programmatic raw logs, predictions, and inferences straight into Arize for immediate visualization and tracking
- **Space & Environment Management** — Browse organizational spaces and segregated deployment environments (Production, Training, Verification)

### How it works

1. Subscribe to this server
2. Enter your Arize API Key and Space ID Key
3. Start monitoring your prediction health from Claude, Cursor, or any MCP-compatible client

No more context-switching into heavily graphical dashboards to figure out why an LLM prompt hallucinated. Your AI acts as a dedicated ML Ops engineer.

### Who is this for?

- **Machine Learning Engineers** — rapidly push inference telemetry and query performance degradation flags without leaving your terminal
- **AI Product Managers** — instantly monitor output toxicity, drift rates, and usage metrics across multiple LLM integrations
- **Data Scientists** — manage baseline evaluation datasets and trigger custom scoring loops asynchronously


## Available Tools
- **list_datasets**: List static evaluation datasets
- **list_environments**: g., Production, Training, Verification) used to segregate model inferences and baseline datasets.

List configured environments within Arize
- **list_evals**: g., Toxicity, Hallucination, PII filtering).

List automated evaluation runs
- **get_dataset**: Get a specific evaluation dataset
- **get_model**: It defines the inputs, outputs, and features.

Get details and metadata for a specific tracked model
- **ingest_log**: payload_json must contain valid Arize payload structures.

Ingest raw telemetry logs into Arize
- **get_metrics**: Fetch observability metrics for an ML model
- **list_models**: List tracked ML models or LLMs
- **run_eval**: Trigger a custom LLM evaluation run
- **list_spaces**: Spaces separate different models and telemetry datasets.

List accessible workspaces within the Arize platform


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Arize AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active Machine Learning models monitored in my workspace."

**🤖 AI Agent:**
> I've fetched your models from the Arize Space. You currently have 3 connected models: 'Fraud-Detection-v2' (Classification), 'Customer-Churn-XGB' (Score), and 'OpenAI-Customer-Service-Bot' (LLM). Would you like to see the recent drift metrics for any of them?

---

**👤 You:**
> "Get the evaluation baseline datasets available for our LLM checks."

**🤖 AI Agent:**
> You have two static evaluation datasets loaded in Arize: 'Support-Tickets-Q2-GroundTruth' (1400 rows) and 'Toxicity-Benchmark' (250 rows). I can trigger an automated `run_eval` check targeting these datasets against your active LLM logs if needed.

---

**👤 You:**
> "Push these 3 mocked prompt responses as telemetry logs to the 'OpenAI-Customer-Service-Bot' model."

**🤖 AI Agent:**
> I successfully structured your 3 prompts into valid ingestion payloads and pushed them via the `ingest_log` tool. They should now be available for analysis and drift observation in the Arize telemetry dashboard.


## Installation & Usage

To install and use the **Arize AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arize-ai](https://vinkius.com/mcp/arize-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
