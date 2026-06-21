# Guru MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/guru)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Manage enterprise knowledge cards, track collections, and search your wiki via AI agents with Guru.

## Description
Connect your **Guru** (Getguru) workspace to any AI agent to automate your knowledge management and enterprise wiki workflows through the Model Context Protocol (MCP). Guru is the AI-powered source of truth that organizes company information into verified cards. This MCP server enables you to retrieve knowledge cards, manage collections, and search your entire workspace directly through natural conversation.

### Key Features

- **Knowledge Card Oversight** — List all knowledge cards, fetch detailed structured content (extended metadata), and create or update cards instantly.
- **Collection Management** — Access and list high-level enterprise groupings (collections) to understand how your knowledge is organized.
- **AI-Powered Search** — Execute powerful searches across all enterprise knowledge silos to isolate answers and verify facts.
- **Board Discovery** — Access board structures that pin collections for specific department or project discovery.
- **Security & Access Control** — List user groups and workspace members to verify knowledge permissions and authorized scopes.
- **Verification Tracking** — Monitor the verification state of your cards to ensure your AI assistant is always using the source of truth.
- **Real-time Synchronization** — Keep your company's collective intelligence accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Guru Email and API Token (found in Team Settings)
3. Start managing your enterprise knowledge from Claude, Cursor, or any MCP client

### Who is this for?

- **Knowledge Managers** — quickly check card verification statuses or update internal wikis without manual dashboard navigation.
- **Customer Support Teams** — get a real-time overview of product documentation and troubleshooting guides via simple AI commands.
- **Internal Operations** — automate the retrieval of company policies and project boards seamlessly.


## Available Tools (12)
- **verify_api_connection**: Check connection
- **create_knowledge_card**: Create new card
- **delete_knowledge_card**: Remove a card
- **get_card_details**: Get card content
- **get_collection_details**: Get collection metadata
- **list_knowledge_boards**: List boards
- **list_knowledge_cards**: List knowledge cards
- **list_knowledge_collections**: List all collections
- **list_access_groups**: List user groups
- **list_workspace_members**: List team members
- **search_knowledge_base**: Search all cards
- **update_knowledge_card**: Modify a card


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Guru** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search my Guru wiki for 'Remote Work Policy'."

**🤖 AI Agent:**
> Searching knowledge base... I found a card titled 'Global Remote Work Policy' in the HR collection. It was last verified 2 days ago. Would you like the full content?

---

**👤 You:**
> "List all my knowledge collections in Guru."

**🤖 AI Agent:**
> Retrieving collections... I found 4 active collections: 'Human Resources' (ID: col_123), 'Engineering Wiki', 'Product Roadmap', and 'Sales Playbook'.

---

**👤 You:**
> "Create a new knowledge card: 'How to setup MCP' in the 'Engineering' collection."

**🤖 AI Agent:**
> Card created! I've successfully added 'How to setup MCP' to the Engineering collection. The card ID is crd_98765 and it is currently in 'Draft' status.


## ❓ FAQ

**Q: How do I get an API Token for Guru?**
Log in to Guru, click your avatar > Team Settings > API Access, and you can generate a new user token there.

**Q: What is a 'Card' in Guru?**
A Card is the fundamental unit of knowledge in Guru. It contains a specific piece of information that can be verified by subject matter experts.

**Q: Can I search for knowledge across all collections?**
Yes! Use the 'search_knowledge_base' tool. It iterates across all enterprise knowledge silos to find relevant cards based on your query.

**Q: How do I find my Collection ID?**
Use the 'list_knowledge_collections' tool. The agent will return all accessible collections along with their unique IDs and names.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/guru](https://vinkius.com/mcp/guru)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Guru** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `guru` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Guru** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "guru": {
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
