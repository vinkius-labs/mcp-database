# MLflow (ML Lifecycle Management) MCP Server

Manage ML lifecycle via MLflow — track training runs, monitor metrics, and audit the model registry.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mlflow-ml-lifecycle-management)

## Overview
**Category:** friends-mcp
**Tools Count:** 6

## Description
Connect your **MLflow** tracking server to any AI agent and take full control of your machine learning experiments, training telemetry, and model registry through natural conversation.

### What you can do

- **Run Orchestration** — Search and retrieve detailed Model Training Runs across specific experiments to track accuracy metrics, loss curves, and scalar parameters directly from your agent
- **Experiment Audit** — List all registered MLflow experiments and retrieve detailed metadata configurations to understand how your project's research branches are structured
- **Metric Inspection** — Extract explicit telemetry capturing the exact state vectors and performance metrics logged during atomic training sessions for rapid diagnostic analysis
- **Model Registry Management** — Search the Global Model Registry to identify models explicitly promoted to production or staging pipelines and track version deployments securely
- **Artifact Visibility** — List physical storage boundaries referencing stored model blobs, image graphs, or metadata saved natively inside MLflow training runs
- **Telemetry Mapping** — Aggregate tracking logs from multiple experiments to identify trends and compare model performance across different historical training sessions

### How it works

1. Subscribe to this server
2. Enter your MLflow Tracking URI and Tracking Token
3. Start managing your ML experiments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists** — monitor training progress and verify model metrics through natural conversation without manual dashboard navigation
- **ML Engineers** — audit the model registry and verify artifact storage locations directly from your workspace terminal
- **AI Operations Teams** — track production model versions and ensure consistent deployment of high-performing ML models efficiently


## Available Tools
- **search_experiments**: Search all MLflow registered Experiments explicitly
- **get_experiment**: Get an explicit explicit MLflow Experiment by ID configuration
- **search_runs**: Search exact Model Training Runs across specific Experiments
- **get_run**: Get parameters and metrics mapping a specific atomic Run ID
- **search_registered_models**: Search the MLflow Global Model Registry
- **list_artifacts**: List static artifacts attached over a specific Run


## Installation & Usage

To install and use the **MLflow (ML Lifecycle Management)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mlflow-ml-lifecycle-management](https://vinkius.com/mcp/mlflow-ml-lifecycle-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
