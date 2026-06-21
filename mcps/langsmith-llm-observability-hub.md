# LangSmith (LLM Observability & Hub) MCP Server

Monitor LLM apps via LangSmith — track traces, audit prompt templates, and manage evaluation datasets.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/langsmith-llm-observability-hub)

## Overview
**Category:** superpower
**Tools Count:** 6

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


## Available Tools
- **list_projects**: Maps out the boundaries of distinct AI pipelines currently monitored by LangSmith.

List all active LangSmith tracing projects/sessions
- **list_runs**: Isolates the raw interactions containing prompts sent to and responses received from the AI models.

List explicit LLM invocation runs within a specific project
- **get_run**: Get precise telemetry for a single LLM invocation run
- **list_datasets**: List all evaluation and fine-tuning datasets mapped in LangSmith
- **list_prompts**: Extract prompt templates hosted in the LangChain Hub
- **list_annotation_queues**: List active human-in-the-loop annotation queues


## Installation & Usage

To install and use the **LangSmith (LLM Observability & Hub)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/langsmith-llm-observability-hub](https://vinkius.com/mcp/langsmith-llm-observability-hub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
