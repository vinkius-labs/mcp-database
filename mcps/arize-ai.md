# Arize AI MCP Server

Automate LLM and ML observability via Arize — monitor models, track telemetry, run evaluations, and analyze data drift directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/arize-ai)

## Overview
**Category:** ai-frontier
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Arize AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arize-ai](https://vinkius.com/mcp/arize-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
