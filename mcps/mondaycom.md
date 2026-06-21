# Monday.com MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mondaycom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage any workflow visually with customizable boards, automations, and dashboards that adapt to how your team actually works.

## Description
Connect your **Monday.com** account to any AI agent and take full control of your team's Work OS through natural conversation. Monday.com provides a flexible and powerful platform for managing complex projects, and this integration allows you to retrieve board metadata, create automated task assignments, and monitor real-time team updates directly from your chat interface.

### What you can do

- **Board & Project Orchestration** — List all managed projects and retrieve detailed column and group metadata programmatically to ensure your team's roadmap is always synchronized.
- **Item Lifecycle Management** — Create, update, and delete board items (tasks) directly from the AI interface to maintain high-fidelity workflow automation.
- **Communication & Update Control** — List and create updates (comments) on specific items via natural language to drive better team alignment and project transparency.
- **User & Workspace Intelligence** — Access platform metadata including user profiles and workspace configurations using simple AI commands.
- **Operational Monitoring** — Track system responses and manage board structures to ensure your team's execution is always optimized.

### How it works

1. Subscribe to this server
2. Enter your Monday.com API Token from your developer settings
3. Start managing your Work OS from Claude, Cursor, or any MCP-compatible client

No more manual logging into the dashboard to check task status or project progress. Your AI acts as a dedicated project coordinator or operations assistant.

### Who is this for?

- **Project Managers & Team Leads** — quickly retrieve project summaries and monitor task health without switching apps.
- **Operations Teams** — automate the creation of tasks and track team capacity via natural conversation.
- **Developers** — integrate real-time project data and board metadata directly within the chat.


## Available Tools
- **create_new_item**: Optional column values must be JSON.

Add row to board
- **post_item_update**: Add comment to row
- **remove_item**: Delete row
- **get_board_schema**: Get board columns
- **get_my_profile**: com user.

Get user info
- **list_boards**: List Monday.com boards
- **list_board_groups**: List board sections
- **list_board_items**: Get board rows
- **list_item_updates**: Get row comments
- **list_account_users**: com account.

List team members
- **list_workspaces**: List project containers
- **update_item_columns**: Modify row values


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Monday.com** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active Monday.com boards in my workspace."

**🤖 AI Agent:**
> I've retrieved your boards. You have 3 active environments: 'Q4 Product Roadmap', 'Team Tasks', and 'Marketing Launch'. Which one would you like to see items for?

---

**👤 You:**
> "Create a new task 'Finalize SEO Audit' in the 'Marketing Launch' board."

**🤖 AI Agent:**
> Task created! I've added 'Finalize SEO Audit' to the Marketing Launch board. Would you like me to assign it to someone or add an initial comment?

---

**👤 You:**
> "Show the latest updates for the 'Acme Corp' item."

**🤖 AI Agent:**
> I've retrieved the updates. The last comment was from Robert Chen: 'Waiting for client approval on the design specs' (2 hours ago).


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific item by its ID?**
Yes! Use the `get_item_details` tool (via queries). Your agent will respond with complete metadata for the record, including column values and update history in seconds.

**Q: How do I find my Monday.com API Token?**
Log in to your Monday.com account, click on your **Avatar** (bottom left), navigate to **Developers**, and you will find your unique secret token under the API section.

**Q: Does this work with private boards?**
Yes, provided the API token used has the necessary permissions and access to those boards within your Monday.com workspace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mondaycom](https://vinkius.com/mcp/mondaycom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Monday.com** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mondaycom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Monday.com** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mondaycom": {
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
