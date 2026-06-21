# Typebot MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/typebot)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Build conversational forms and chatbot flows with a beautiful open-source visual editor that creates engaging user experiences.

## Description
Connect your **Typebot** account to any AI agent and simplify how you build, manage, and analyze your conversational assistants through natural conversation.

### What you can do

- **Bot Management** — List all typebots across your workspaces and folders, and retrieve detailed metadata and flow structures.
- **Deployment Control** — Publish the latest bot changes to production instantly without leaving your agent.
- **Result Analysis** — List and export user submissions and conversation results to track leads and performance.
- **Organization Oversight** — Manage workspaces and folders to keep your conversational projects structured.
- **Session Testing** — Programmatically start new chat sessions to verify bot logic and user experiences.

### How it works

1. Subscribe to this server
2. Enter your Typebot API Token (found in your account settings)
3. Start managing your conversational forms from Claude, Cursor, or any MCP client

### Who is this for?

- **Conversation Designers** — quickly verify bot logic and publish updates via simple AI commands.
- **Marketing & Sales Teams** — monitor incoming results and export lead data directly from the workspace.
- **Product Managers** — get instant bird's-eye views of bot performance and organization folders via the AI assistant.


## Available Tools
- **delete_typebot**: Permanently delete a typebot
- **get_typebot_details**: Essential for reviewing the bot logic.

Get details and structure for a specific typebot
- **list_typebots**: Can be filtered by a specific workspace ID.

List all conversational typebots
- **list_folders**: Folders are used to group related typebots.

List all folders in a workspace
- **list_typebot_results**: Essential for data analysis and lead export.

List collected user responses for a bot
- **list_workspaces**: Workspaces contain folders and bots.

List all accessible Typebot workspaces
- **publish_typebot**: Requires the unique bot ID.

Publish and deploy the latest bot changes
- **start_chat_session**: Useful for testing bot flows or automated interactions.

Programmatically start a new bot conversation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Typebot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all typebots in my current workspace."

**🤖 AI Agent:**
> I've retrieved your typebots. You have 3 active bots: 'Lead Gen Flow', 'Customer Survey v2', and 'Support Assistant'. Which one would you like to publish or analyze?

---

**👤 You:**
> "Show me the collected results for the 'Lead Gen Flow' bot."

**🤖 AI Agent:**
> I've fetched the results. There are 15 recent submissions including leads from 'John Doe' (john@example.com) and 'Sarah Smith'. Shall I retrieve the detailed answers for any of them?

---

**👤 You:**
> "Publish the latest changes for bot 'bot_10293'."

**🤖 AI Agent:**
> Success! The latest changes for bot bot_10293 have been published to production. Your conversational form is now up-to-date at its public URL.


## ❓ FAQ

**Q: Can I publish a bot after making changes via AI?**
Yes! Use the `publish_typebot` action and provide the unique bot ID. Your agent will instantly deploy the latest changes to the public URL.

**Q: How do I see the submissions or leads collected by a bot?**
Run the `list_typebot_results` query with your Typebot ID. The agent will retrieve the complete history of user responses and collected data.

**Q: Is it possible to list bots from a specific workspace?**
Absolutely. Use the `list_typebots` tool and provide the optional `workspace_id` to retrieve only the bots associated with that team area.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/typebot](https://vinkius.com/mcp/typebot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Typebot** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `typebot` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Typebot** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "typebot": {
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
