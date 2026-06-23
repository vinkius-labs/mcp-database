# Pinata Cloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pinata-cloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate IPFS pinning and decentralized storage via Pinata — manage files, JSON, and groups directly with AI.

## Description
Connect your **Pinata Cloud** account to any AI agent and take full control of your decentralized storage and IPFS orchestration through natural conversation. Pinata is the premier platform for Web3 content management, and this integration allows you to pin files, manage decentralized metadata, and organize content into groups directly from your chat interface.

### What you can do

- **IPFS Pinning Orchestration** — Pin files and JSON objects programmatically to the decentralized web and retrieve their unique CIDs (Content Identifiers) instantly.
- **Decentralized Metadata Control** — Update pin names and key-values via natural language to maintain a high-fidelity catalog of your decentralized assets.
- **Storage & Group Intelligence** — Create and manage organizational groups and retrieve detailed pin lists with technical filters directly from the AI interface.
- **Usage & API Oversight** — Monitor account data usage, manage API keys, and verify authentication health using simple AI commands.
- **Operational Monitoring** — Track system responses and manage unpinning workflows to ensure your storage strategy is always optimized.

### How it works

1. Subscribe to this server
2. Enter your Pinata JWT (JSON Web Token) from your API keys settings
3. Start managing your decentralized content from Claude, Cursor, or any MCP-compatible client

No more manual dashboard uploading or CID tracking. Your AI acts as a dedicated Web3 architect or decentralized storage manager.

### Who is this for?

- **NFT Creators & Developers** — quickly pin metadata assets and monitor IPFS availability without switching apps.
- **Web3 Engineering Teams** — automate the organization of decentralized storage and track usage via natural conversation.
- **Data Architects** — streamline the retrieval of decentralized content metadata and monitor organizational health directly within the chat.


## Available Tools (12)
- **create_pin_group**: Add new collection
- **remove_pin_group**: Delete collection
- **get_pinning_stats**: Check data usage
- **get_group_details**: Get group info
- **list_pin_groups**: List pin collections
- **list_api_keys**: List account keys
- **list_ipfs_pins**: List pinned files
- **pin_json_to_ipfs**: Pin NFT metadata/JSON
- **revoke_api_key**: Disable an API key
- **verify_pinata_auth**: Check connection
- **remove_ipfs_pin**: Unpin file/hash
- **update_pin_metadata**: Modify pin name/tags


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pinata Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 files pinned to IPFS."

**🤖 AI Agent:**
> I've retrieved your recent pins. You have 5 files including 'Profile_Avatar.png' (CID: Qm...) and 'Project_Metadata.json'. Would you like me to create a group for these?

---

**👤 You:**
> "Upload and pin my application metadata JSON to IPFS with a custom name for easy retrieval."

**🤖 AI Agent:**
> File pinned to IPFS successfully. CID: bafkreihdwdcefgh4dqkjv67uzcmw7ojee6xedzdetojuzjevtenrj. Name: "app-metadata-v2.json". Size: 4.2 KB. Gateway URL: gateway.pinata.cloud/ipfs/bafkrei... The content is now permanently available on the IPFS network and accessible through any IPFS gateway. Pin status: Pinned across 3 nodes for redundancy.

---

**👤 You:**
> "List all my pinned files on IPFS and check which ones are consuming the most storage."

**🤖 AI Agent:**
> You have 47 pinned files using 2.3 GB of your 5 GB plan. Top 5 by size: "nft-collection-images.zip" (890 MB), "video-assets-q2.mp4" (456 MB), "product-catalog.json" (234 MB), "user-avatars-batch.tar" (178 MB), "brand-guidelines.pdf" (89 MB). 12 files were pinned in the last 30 days. 8 files have not been accessed in over 90 days and could be candidates for unpinning.


## ❓ FAQ

**Q: Can my AI automatically find the CID (hash) of a specific pinned file?**
Yes! Use the `list_pins` tool. Provide filters like the pin name, and your agent will respond with the unique IPFS hash (CID) and associated technical metadata in seconds.

**Q: How do I find my Pinata JWT?**
Log in to Pinata, navigate to **API Keys**, click **New Key**, and ensure you select all **Admin** permissions. Copy the long **JWT** string provided at the end.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pinata-cloud](https://vinkius.com/mcp/pinata-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pinata Cloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pinata-cloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pinata Cloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pinata-cloud": {
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
