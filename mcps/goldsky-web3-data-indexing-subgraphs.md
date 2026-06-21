# Goldsky (Web3 Data Indexing & Subgraphs) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/goldsky-web3-data-indexing-subgraphs)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/goldsky-web3-data-indexing-subgraphs-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/goldsky-web3-data-indexing-subgraphs-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage Web3 data pipelines and subgraphs. List, create, and monitor real-time indexing pipelines directly from your AI agent.

## Description
Connect your **Goldsky** account to any AI agent to orchestrate high-performance Web3 data pipelines through natural language. Goldsky provides the infrastructure to index blockchain data in real-time, and this MCP server puts that power in your chat interface.

### What you can do

- **Pipeline Management** — List all active Turbo pipelines, create new ones from JSON definitions, and delete obsolete ones.
- **Lifecycle Control** — Pause, resume, or restart pipelines instantly to manage resource usage or apply updates.
- **Real-time Monitoring** — Fetch execution logs, check runtime status (running, paused, failed), and inspect internal pipeline states.
- **Error Tracking** — Query error counts within specific time windows to ensure your data indexing remains healthy.
- **Validation** — Validate pipeline definitions (sources, transforms, sinks) before deployment to prevent configuration errors.

### How it works

1. Subscribe to this server
2. Enter your Goldsky API Key
3. Start managing your Web3 data infrastructure from Claude, Cursor, or any MCP client

### Who is this for?

- **Web3 Developers** — Deploy and debug subgraphs and pipelines without leaving your code editor.
- **Data Engineers** — Monitor indexing health and retrieve logs to troubleshoot data flow issues in real-time.
- **Protocol Teams** — Manage cross-chain data indexing infrastructure through simple conversational commands.


## Available Tools
- **create_pipeline**: Create and deploy a new pipeline
- **delete_pipeline**: Delete a pipeline (irreversible)
- **get_pipeline_error_count**: Get error count in a time window for a pipeline
- **get_pipeline_logs**: Retrieve execution logs for a pipeline
- **get_pipeline_state**: Get internal state of a pipeline
- **get_pipeline_status**: g., running, paused, failed) of a pipeline.

Get current runtime status of a pipeline
- **get_pipeline**: Get details of a specific pipeline
- **list_pipelines**: List all pipelines in the project
- **pause_pipeline**: Pause a running pipeline
- **restart_pipeline**: Restart a pipeline
- **resume_pipeline**: Resume a paused pipeline
- **validate_pipeline**: Validate a pipeline definition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Goldsky (Web3 Data Indexing & Subgraphs)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active Goldsky pipelines."

**🤖 AI Agent:**
> I've retrieved your pipelines. You have 3 active: 'eth-mainnet-swaps', 'polygon-nft-events', and 'base-bridge-monitor'. Which one would you like to inspect?

---

**👤 You:**
> "Check the status and error count for the pipeline 'eth-mainnet-swaps'."

**🤖 AI Agent:**
> The pipeline 'eth-mainnet-swaps' is currently 'RUNNING'. I detected 0 errors in the last time window. Everything looks healthy.

---

**👤 You:**
> "Show me the recent logs for the 'polygon-nft-events' pipeline."

**🤖 AI Agent:**
> Fetching logs for 'polygon-nft-events'... [INFO] Successfully indexed block 5420123... [INFO] Processed 12 Transfer events... [DEBUG] Sink connection stable.


## Installation & Usage

To install and use the **Goldsky (Web3 Data Indexing & Subgraphs)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/goldsky-web3-data-indexing-subgraphs](https://vinkius.com/mcp/goldsky-web3-data-indexing-subgraphs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
