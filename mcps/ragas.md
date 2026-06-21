# Ragas MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ragas)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ragas-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ragas-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Equip your AI with Ragas to create datasets, run RAG evaluations, and track experiment metrics directly from your workflow.

## Description
Integrate **Ragas** with your AI agent to bring professional grade RAG (Retrieval-Augmented Generation) evaluation and tracking into your chat interface. By subscribing to this server, the AI can seamlessly manage datasets and measure LLM performance on demand.

### What you can do

- **Dataset Management** — Upload, list, and organize evaluation datasets directly inside your environment.
- **Run Evaluations** — Automatically trigger Ragas evaluations on your RAG pipelines and fetch detailed scoring.
- **Track Experiments** — Monitor and compare iterative improvements by viewing tracked metrics across different agent versions.
- **Project Organization** — Associate evaluations with specific projects within your Ragas dashboard.

### How it works

1. Enable the server integration.
2. Provide your Ragas Application URL and your generated Application Token.
3. Instruct your AI to initiate evaluations or query historical metrics natively from your IDE or chat.

### Who is this for?

- **AI & ML Engineers** — Run pipeline evaluations without context switching to a separate dashboard or writing Python evaluation scripts each time.
- **QA Specialists for LLMs** — Rapidly examine datasets and benchmark results to ensure hallucination rates remain low.
- **Data Scientists** — Compare multiple RAG configuration experiments side-by-side using unified metrics.


## Available Tools
- **list_datasets**: Lists available evaluation datasets
- **get_dataset**: Retrieves details for a specific evaluation dataset
- **list_experiments**: Lists experiments associated with a specific dataset
- **get_experiment**: Retrieves detailed information for a specific experiment
- **run_evaluation**: g., faithfulness, answer_relevancy).

Triggers a new evaluation run for a dataset
- **list_metrics**: Lists all available evaluation metrics
- **get_results**: Retrieves the results of a completed experiment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ragas** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Ragas datasets available in my project."

**🤖 AI Agent:**
> Using the `list_datasets` command, I found 3 datasets: 'Legal_Q1_Test' (ID: 01), 'Medical_V2_Base' (ID: 02), and 'General_FAQ_Validation' (ID: 03).

---

**👤 You:**
> "Fetch the metrics and results for the recent experiment 'Support Bot V3'."

**🤖 AI Agent:**
> Looking up experiments... For 'Support Bot V3', the evaluation scored an aggregate 0.89. Faithfulness scored 0.92, while Answer Relevance was slightly lower at 0.85.

---

**👤 You:**
> "Create a new Ragas project named 'Financial_RAG_Testing'."

**🤖 AI Agent:**
> I executed `create_project`. The project 'Financial_RAG_Testing' has been successfully created and initialized on your Ragas dashboard.


## Installation & Usage

To install and use the **Ragas** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ragas](https://vinkius.com/mcp/ragas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
