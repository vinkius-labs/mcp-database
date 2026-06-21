# Filebase (Web3 Storage) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/filebase-web3-storage)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage decentralized storage on IPFS via Filebase — upload files, pin CIDs, manage IPNS names, and track storage usage directly from any AI agent.

## Description
Connect your **Filebase** account to any AI agent and take full control of your decentralized Web3 storage workflows through natural conversation.

### What you can do

- **IPFS Operations** — Add text files, fetch content by CID, and manage raw blocks directly on the IPFS network using the RPC API.
- **Pinning Management** — Use the Pinning Service API (PSA) or RPC to pin, list, and remove content identifiers (CIDs) for persistent storage.
- **IPNS & Keys** — Generate keypairs, publish CIDs to IPNS, and resolve names to IPFS paths for mutable decentralized websites.
- **Usage & Infrastructure** — Monitor storage usage, manage dedicated gateways, and track bucket metrics across the platform.

### How it works

1. Subscribe to this server
2. Enter your Filebase API Key and Platform Token
3. Start managing your Web3 assets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — interact with IPFS and IPNS directly from your coding environment without switching to CLI or web dashboards.
- **DevOps Engineers** — automate pinning and storage monitoring as part of your infrastructure workflows.
- **Content Creators** — manage decentralized assets and metadata for NFTs or dApps using simple natural language commands.


## Available Tools (29)
- **platform_create_gateway**: Create a new dedicated gateway
- **platform_create_name**: Create a new IPNS name
- **platform_delete_gateway**: Delete a dedicated gateway
- **platform_delete_name**: Delete an IPNS name
- **platform_get_bucket_usage**: Get storage usage for a specific bucket
- **platform_get_gateway**: Get details of a specific dedicated gateway
- **platform_get_gateway_usage**: Get bandwidth usage for a dedicated gateway
- **platform_get_name**: Get details of a specific IPNS name
- **platform_get_usage**: Get total storage and bandwidth usage
- **platform_list_gateways**: List all dedicated gateways
- **platform_list_names**: List all IPNS names
- **platform_update_gateway**: Update a dedicated gateway
- **platform_update_name**: Update an IPNS name to point to a new CID
- **psa_add_pin**: Add a pin using the Pinning Service API
- **psa_get_pin**: Get pin status by request ID
- **psa_list_pins**: List pins using the Pinning Service API
- **psa_remove_pin**: Remove a pin by request ID
- **psa_replace_pin**: Replace an existing pin
- **rpc_add**: Add a text file to IPFS
- **rpc_block_get**: Retrieve a raw block by CID
- **rpc_cat**: Fetch contents of a file by CID
- **rpc_key_gen**: Create a new keypair
- **rpc_key_list**: List all keys in the keychain
- **rpc_name_publish**: Publish a CID to IPNS
- **rpc_name_resolve**: Resolve an IPNS name to an IPFS path
- **rpc_pin_add**: Pin a CID to persistent storage
- **rpc_pin_ls**: List all pinned objects via RPC
- **rpc_pin_rm**: Unpin a CID via RPC
- **rpc_version**: Get the version of the IPFS daemon


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Filebase (Web3 Storage)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Upload the text 'Hello from Filebase MCP' to IPFS."

**🤖 AI Agent:**
> I've uploaded your text to IPFS. The generated CID is `QmXoyp...`. You can now access this content or pin it for long-term storage.

---

**👤 You:**
> "Show me a list of all my pinned objects."

**🤖 AI Agent:**
> Fetching your pinned objects... I found 12 active pins. The most recent ones include `Qm...` (Status: pinned) and `bafy...` (Status: pinning).

---

**👤 You:**
> "What is my current storage usage on Filebase?"

**🤖 AI Agent:**
> Your current usage is 4.2 GB out of your 10 GB limit. You have used 150 MB of bandwidth this month across 3 active buckets.


## ❓ FAQ

**Q: How do I pin a specific CID to ensure it stays on the network?**
You can use the `rpc_pin_add` tool by providing the CID. This ensures the content is persistently stored on Filebase's IPFS infrastructure.

**Q: Can I check my current storage usage and limits?**
Yes! Use the `platform_get_usage` tool. It will return your total storage used, bandwidth metrics, and current subscription limits.

**Q: How do I publish a CID to a mutable IPNS name?**
Use the `rpc_name_publish` tool with the target CID. This maps your content to an IPNS address that stays the same even when the content updates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/filebase-web3-storage](https://vinkius.com/mcp/filebase-web3-storage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Filebase (Web3 Storage)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `filebase-web3-storage` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Filebase (Web3 Storage)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "filebase-web3-storage": {
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
