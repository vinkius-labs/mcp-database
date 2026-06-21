# Dataiku DSS MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dataiku-dss)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dataiku-dss-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dataiku-dss-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Manage data science via Dataiku — list projects and datasets, track pipeline jobs, run automation scenarios, and monitor ML models directly from any AI agent.

## Description
Connect your **Dataiku DSS** instance to any AI agent and take full control of your enterprise AI and collaborative data science workflows through natural conversation.

### What you can do

- **Project & Dataset Exploration** — List all accessible DSS projects and retrieve structural extraction of dataset column schemas and types
- **Pipeline Orchestration** — Monitor build tasks and training runs by listing pipeline jobs and analyzing execution states and timing
- **Transformation Auditing** — Retrieve explicit configuration structures parsing precise Dataiku recipes (Python, SQL, Visual) to verify data logic
- **Automation & Scenarios** — List automation scenarios and trigger execution commands to rebuild pipelines or retrain models securely
- **Model Monitoring** — Identify saved ML models and retrieve detailed performance metrics defining specific trained schema layers
- **Admin Oversight** — Enumerate installed plugins and data connections (SQL, Cloud Storage, APIs) to verify organizational constraints

### How it works

1. Subscribe to this server
2. Enter your Dataiku Instance URL and API Key (Personal, Project, or Global key)
3. Start managing your data science workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists** — monitor model training and compare dataset schemas without leaving the research flow
- **Data Engineers** — track pipeline jobs and verify recipe configurations using natural language
- **MLOps Teams** — trigger automation scenarios and monitor deployed models in real-time
- **Analytics Managers** — audit project metadata and data connections across the organization


## Available Tools
- **list_projects**: List all DSS projects accessible to the API key
- **get_project**: Get project metadata, settings, and tags
- **list_datasets**: List all datasets in a project
- **dataset_schema**: Get the schema (columns, types) of a specific dataset
- **list_recipes**: List all recipes (data transformations) in a project
- **get_recipe**: Get recipe configuration and settings
- **list_jobs**: List pipeline jobs in a project (build tasks, training runs)
- **get_job**: Get job state, timing, and outputs
- **list_scenarios**: List automation scenarios in a project
- **run_scenario**: Trigger a scenario execution (build pipeline, retrain model)
- **list_models**: List deployed/saved ML models in a project
- **get_model**: Get saved model metadata, algorithm, and performance metrics
- **list_plugins**: List installed DSS plugins
- **list_connections**: List all DSS data connections (databases, cloud storage, APIs)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dataiku DSS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all projects in my Dataiku instance"

**🤖 AI Agent:**
> I found 5 projects: 'Churn-Prediction-Q1', 'Customer-Segmentation', 'Fraud-Detection-Live', 'Sales-Forecasting', and 'Staging-Sandbox'. Which one would you like to explore?

---

**👤 You:**
> "What is the schema for dataset 'raw_logs' in project 'FRAUD'?"

**🤖 AI Agent:**
> Retrieving schema for 'raw_logs'... It contains 12 columns including 'timestamp' (date), 'user_id' (string), 'ip_address' (string), and 'action_type' (string). I can provide the full type mapping if you'd like.

---

**👤 You:**
> "Run scenario 'REBUILD_PIPELINE' in project 'SALES'"

**🤖 AI Agent:**
> Scenario triggered! 'REBUILD_PIPELINE' is now executing in project 'SALES'. The system is rebuilding the underlying datasets and recipes. I will notify you once the run is complete.


## Installation & Usage

To install and use the **Dataiku DSS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dataiku-dss](https://vinkius.com/mcp/dataiku-dss)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
