# Medium MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/medium)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [content-management](../categories/content-management.md)

Publish and manage content on Medium — create posts and manage publications directly from any AI agent.

## Description
Connect your **Medium** account to any AI agent and automate your publishing workflow through natural conversation.

### What you can do

- **Post Creation** — Quickly publish public articles or save drafts directly to your Medium account
- **Publication Management** — List publications you belong to and publish content directly under their brand
- **Profile Inspection** — Retrieve your unique User ID and profile details for seamless integration
- **Contributor Lists** — View authorized contributors for publications you manage

### How it works

1. Subscribe to this server
2. Enter your Medium Integration Token
3. Start publishing from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **create_draft**: Create a new draft
- **create_post**: Create a new post for a user
- **create_public_post**: Create a public post
- **create_publication_post**: Create a post under a publication
- **get_authenticated_user**: Get details for the authenticated user
- **get_my_user_id**: Get your User ID
- **get_my_profile**: Get your own profile
- **list_contributors**: List contributors for a publication
- **list_my_publications**: List your own publications
- **list_publications**: List publications for a user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Medium** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show my Medium profile and user ID."

**🤖 AI Agent:**
> Retrieving your profile... You are logged in as '@username' (ID: 12345).

---

**👤 You:**
> "Create a draft titled 'My AI Journey' with content 'This is my first post...'"

**🤖 AI Agent:**
> Draft created successfully! You can view and edit it on Medium. URL: https://medium.com/p/draft-id

---

**👤 You:**
> "List my publications."

**🤖 AI Agent:**
> Searching... You are a member of 2 publications: 'The Startup' and 'UX Collective'.


## ❓ FAQ

**Q: How do I get a Medium Integration Token?**
Go to Medium Settings > Security and apps > Integration tokens to generate your token.

**Q: Can I publish in Markdown?**
Yes! The `create_post` and `create_draft` tools support Markdown format natively.

**Q: Is my token secure?**
Absolutely. Your token is encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/medium](https://vinkius.com/mcp/medium)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Medium** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `medium` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Medium** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "medium": {
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
