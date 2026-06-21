# Langfuse (LLM Tracing & Evals) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/langfuse-llm-tracing-evals)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/langfuse-llm-tracing-evals-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/langfuse-llm-tracing-evals-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Monitor LLM apps via Langfuse — track traces, manage prompt templates, and audit evaluation scores.

## Description
Connect your **Langfuse** account to any AI agent and take full control of your LLM observability, prompt management, and quality evaluation through natural conversation.

### What you can do

- **Trace Orchestration** — List and retrieve detailed traces of LLM API sessions, exposing latencies, token counts, and exact chained payloads directly from your agent
- **Prompt Vault Access** — Query actively managed prompt templates and versions to inspect system instructions and expected input variables
- **Observation Analysis** — Deep-dive into individual spans, events, and generations within a trace to pinpoint failures or performance bottlenecks securely
- **Evaluation & Scoring** — Attach structured human feedback or automated evaluation metrics to specific traces to monitor model grounding and accuracy
- **Usage Metrics** — Generate aggregated daily reports on USD costs and average latency to track your AI infrastructure spending in real-time
- **Session Monitoring** — Extract correlated user sessions to understand multi-turn interaction boundaries and improve long-term agentic workflows

### How it works

1. Subscribe to this server
2. Enter your Langfuse API URL, Public Key, and Secret Key
3. Start monitoring your LLM application from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **LLM Engineers** — debug complex AI chains and measure exact token latencies through natural conversation without manual dashboard searching
- **Product Owners** — monitor daily AI costs and user satisfaction scores across multiple production environments
- **Data Scientists** — manage prompt templates and audit evaluation metrics to improve model response quality and grounding efficiently


## Available Tools
- **get_trace**: Get complete telemetry and nested graph for a single trace
- **get_daily_metrics**: Generate rolled-up USD cost and aggregated latency statistics
- **create_observation**: Create a new LLM observation (span, event, generation) inside a trace
- **get_observation**: Retrieve explicit span or generation context within a trace
- **list_observations**: List raw observation objects spanning across traces
- **list_prompts**: Extract actively managed prompt templates and versions
- **create_score**: g. 1-5 stars) or automated pipeline metrics bounding exactly onto the specified Trace or Observation.

Attach human feedback or evaluation metrics to a trace/observation
- **list_scores**: List all explicit scores mapping quality or cost algorithms
- **list_sessions**: List high-level user session entities encapsulating multiple traces
- **list_traces**: List all traces tracking LLM API sessions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Langfuse (LLM Tracing & Evals)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 traces in my Langfuse project"

**🤖 AI Agent:**
> I've retrieved the latest 5 traces. Highlights include 'Email-Summarization' (Latency: 1.2s, 450 tokens), 'Chat-Interaction-987' (Latency: 2.4s, 1,200 tokens), and 'Data-Extraction-Fail' (Status: Error). Would you like to inspect the error payload for the failed trace?

---

**👤 You:**
> "Show me the instructions for the 'customer-support-v3' prompt"

**🤖 AI Agent:**
> Retrieving 'customer-support-v3'… The system instruction is: 'You are a helpful support agent for TechCorp. Answer queries based on the provided documentation…'. It expects variables: 'customer_name' and 'query_text'. Would you like to see the previous versions?

---

**👤 You:**
> "What was our total LLM spending for today?"

**🤖 AI Agent:**
> Your total LLM spending for today is $12.45 across 45,200 total tokens. The average latency is 1.8s. The most expensive model remains 'gpt-4-turbo' with $8.20 in costs. I can provide a breakdown by provider if needed.


## Installation & Usage

To install and use the **Langfuse (LLM Tracing & Evals)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/langfuse-llm-tracing-evals](https://vinkius.com/mcp/langfuse-llm-tracing-evals)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
