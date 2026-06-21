# Theta MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/theta)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Interact with Theta Network — query blockchain data, manage AI EdgeCloud deployments, and orchestrate decentralized video delivery.

## Description
Connect to the **Theta Network** ecosystem to manage decentralized infrastructure directly through your AI agent. This server provides comprehensive tools for blockchain interaction, video processing, and EdgeCloud AI resource management.

### What you can do

- **Blockchain Operations** — Query account balances, fetch block details by hash or height, and inspect transactions or pending mempool data using standard RPC calls.
- **EdgeCloud AI** — List standard templates, check available VM resources, and manage the full lifecycle of AI deployments (create, start, stop, delete).
- **Decentralized Video** — Create upload URLs, transcode assets, manage livestreams, and search through video libraries using Theta's specialized video infrastructure.
- **Key Management** — List local account addresses and manage encrypted keys via the Theta CLI integration.

### How it works

1. Subscribe to this server
2. Provide your Theta RPC URL and EdgeCloud/Video API credentials
3. Start querying the blockchain or deploying AI models from Claude, Cursor, or any MCP client

### Who is this for?

- **Web3 Developers** — interact with the Theta blockchain and smart contracts without leaving your coding environment
- **AI Engineers** — automate the deployment and scaling of models on Theta's decentralized EdgeCloud
- **Content Platforms** — manage video workflows and livestreams programmatically via natural language


## Available Tools (30)
- **ai_create_deployment**: Launch a new AI model or Jupyter Notebook
- **ai_delete_deployment**: Delete an AI deployment
- **ai_list_deployments**: List all deployments in a project
- **ai_list_standard_templates**: List built-in AI templates
- **ai_list_vm_resources**: g., vm_gt1 for NVIDIA T4).

List available machine types
- **ai_start_deployment**: Restart a stopped GPU Node
- **ai_stop_deployment**: Stop a running GPU Node
- **cli_list_keys**: List local account addresses
- **cli_lock_key**: Lock local accounts
- **cli_new_key**: Create a new encrypted account locally
- **cli_send**: Send Theta/TFuel
- **cli_unlock_key**: Unlock a local account for sending
- **rpc_get_account**: Get Theta account details
- **rpc_get_block_by_height**: Get finalized block at a given height
- **rpc_get_block**: Get block details by hash
- **rpc_broadcast_raw_transaction_async**: Submit a signed transaction asynchronously
- **rpc_broadcast_raw_transaction**: Submit a signed transaction synchronously
- **rpc_call_smart_contract**: Simulate a smart contract execution locally
- **rpc_get_pending_transactions**: Get pending transactions
- **rpc_get_transaction**: Get transaction details by hash
- **rpc_get_version**: Get Theta blockchain version
- **video_create_livestream**: Create a livestream object
- **video_create_upload_url**: Create a Video Upload URL
- **video_get**: Get video details
- **video_list_ingestors**: List available Edge Ingestors
- **video_list**: List all videos for a service account
- **video_search**: Search videos by metadata
- **video_select_ingestor**: Assign an ingestor to a stream
- **video_transcode**: Transcode a video
- **video_unselect_ingestor**: Release an ingestor


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Theta** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current version of the Theta blockchain software?"

**🤖 AI Agent:**
> I've checked the network status. The current Theta blockchain version is v4.2.0.

---

**👤 You:**
> "List all available VM resources for AI deployments on EdgeCloud."

**🤖 AI Agent:**
> I've retrieved the available VM resources. You have access to several tiers including 'Small' (2 vCPU, 4GB RAM) and 'GPU-Medium' (NVIDIA T4, 16GB RAM).

---

**👤 You:**
> "Show me the details for block height 25000000."

**🤖 AI Agent:**
> Fetching block 25000000... The block hash is 0xabc... and it contains 12 transactions. It was finalized at timestamp 1712345678.


## ❓ FAQ

**Q: How can I check the balance and sequence of a specific Theta wallet?**
Use the `rpc_get_account` tool by providing the wallet address (0x...). The agent will return the coin balances and the current sequence number for that account.

**Q: Can I manage AI model deployments on Theta EdgeCloud?**
Yes. You can use `ai_list_deployments` to see active ones, and `ai_create_deployment` or `ai_stop_deployment` to control your AI infrastructure resources.

**Q: How do I search for existing video assets in my Theta library?**
Simply use the `video_search` tool. You can provide a query string to filter through your uploaded and transcoded video content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/theta](https://vinkius.com/mcp/theta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Theta** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `theta` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Theta** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "theta": {
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
