# Akash Network (Decentralized GPU & Cloud API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/akash-network-decentralized-gpu-cloud-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/akash-network-decentralized-gpu-cloud-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/akash-network-decentralized-gpu-cloud-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Deploy and manage decentralized GPU and cloud resources on Akash Network—create deployments, manage leases, and monitor escrow balances directly.

## Description
Connect to **Akash Network**, the world's first decentralized open-source cloud, through your AI agent. This server allows you to orchestrate high-performance computing resources, including GPUs for AI training and inference, using natural language.

### What you can do

- **Deployment Management** — Create, update, and close deployments using standard SDL (Stack Definition Language) manifests.
- **Bidding & Leases** — Poll for provider bids and create leases to secure your compute resources at competitive prices.
- **Financial Control** — Monitor escrow balances and add USD deposits to keep your services running without interruption.
- **Automation** — Enable and configure auto top-up settings to ensure your decentralized infrastructure scales with your needs.
- **Resource Inspection** — Retrieve full details of active leases and deployment statuses to maintain high availability.

### How it works

1. Subscribe to this server
2. Enter your Akash API Key
3. Start deploying decentralized infrastructure via Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Researchers** — Spin up high-end GPUs for model training or inference without the overhead of centralized cloud providers.
- **DevOps Engineers** — Manage decentralized infrastructure using familiar SDL manifests directly from your IDE.
- **Web3 Developers** — Build and host dApps on a truly decentralized cloud with automated resource management.


## Available Tools
- **add_deposit**: Add USD funds to a deployment escrow
- **close_deployment**: Close a deployment
- **create_deployment**: 50 USD).

Create a new deployment from an SDL manifest
- **create_lease**: Accept bids and create a lease
- **enable_auto_top_up**: Enable auto top-up for deployments
- **get_deployment_settings**: Get auto top-up settings for a deployment
- **get_deployment**: Get full details of a deployment
- **get_provider**: Get details for a specific provider
- **list_bids**: Bids typically arrive in 30-60 seconds.

Poll for provider bids for a deployment
- **list_deployments**: List all deployments
- **list_providers**: List network-wide providers
- **update_deployment_settings**: Update deployment settings
- **update_deployment**: Update an active deployment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Akash Network (Decentralized GPU & Cloud API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active deployments on Akash."

**🤖 AI Agent:**
> I've retrieved your deployments. You have 2 active workloads: 'AI-Training-Cluster' (DSEQ: 105542) and 'Web-App-Node' (DSEQ: 105548). Would you like to check the escrow balance for either of them?

---

**👤 You:**
> "Add a $10 deposit to deployment 105542."

**🤖 AI Agent:**
> Processing deposit... I have successfully added $10.00 USD to the escrow for DSEQ 105542. The new balance is now $14.50 USD, extending your estimated runtime.

---

**👤 You:**
> "Close the deployment with DSEQ 105548."

**🤖 AI Agent:**
> Closing deployment... DSEQ 105548 has been successfully closed. Associated resources have been released and the remaining escrow balance will be returned to your account.


## Installation & Usage

To install and use the **Akash Network (Decentralized GPU & Cloud API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/akash-network-decentralized-gpu-cloud-api](https://vinkius.com/mcp/akash-network-decentralized-gpu-cloud-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
