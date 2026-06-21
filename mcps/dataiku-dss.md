# Dataiku DSS MCP Server

Manage data science via Dataiku — list projects and datasets, track pipeline jobs, run automation scenarios, and monitor ML models directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dataiku-dss)

## Overview
**Category:** ai-frontier
**Tools Count:** 14

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


## Installation & Usage

To install and use the **Dataiku DSS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dataiku-dss](https://vinkius.com/mcp/dataiku-dss)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
