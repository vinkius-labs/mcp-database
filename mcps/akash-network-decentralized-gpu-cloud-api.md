# Akash Network (Decentralized GPU & Cloud API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/akash-network-decentralized-gpu-cloud-api)
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


## Available Tools (13)
- **close_deployment**: Close a deployment
- **add_deposit**: Add USD funds to a deployment escrow
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


## ❓ FAQ

**Q: How do I check for available provider bids after creating a deployment?**
Use the `list_bids` tool with your deployment's DSEQ. It typically takes 30-60 seconds for providers to submit bids for your workload.

**Q: Can I update a running deployment with a new SDL manifest?**
Yes! Use the `update_deployment` tool. Provide the existing DSEQ and your revised SDL string to apply changes to your active resources.

**Q: How do I prevent my deployment from closing due to insufficient funds?**
You can use `add_deposit` to manually add USD to the escrow, or use `enable_auto_top_up` to configure automatic funding based on your deployment's needs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/akash-network-decentralized-gpu-cloud-api](https://vinkius.com/mcp/akash-network-decentralized-gpu-cloud-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Akash Network (Decentralized GPU & Cloud API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `akash-network-decentralized-gpu-cloud-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Akash Network (Decentralized GPU & Cloud API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "akash-network-decentralized-gpu-cloud-api": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
