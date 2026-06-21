# Pivotal Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pivotal-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage agile projects via Pivotal Tracker — list stories, track epics, and update tasks directly from any AI agent.

## Description
Connect your **Pivotal Tracker** workspace to any AI agent and take full control of your agile development workflows through natural conversation.

### What you can do

- **Story Management** — List, retrieve, create, and update stories (features, bugs, chores) across your projects.
- **Project Oversight** — List all projects and retrieve detailed metadata to maintain visibility over your workspace.
- **Epic & Label Tracking** — List epics and labels to understand the high-level progress and categorization of your work.
- **Team Visibility** — List project memberships to see who is working on what.
- **Profile Access** — Retrieve your own profile information to verify your current account context.

### How it works

1. Subscribe to this server
2. Enter your Pivotal Tracker API Token (from Profile Settings)
3. Start managing your backlog directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Agile Product Owners** — quickly check the status of a story or update the backlog while reviewing requirements.
- **Software Engineers** — update story states (started, finished, delivered) or check epic progress without leaving the IDE.
- **Project Managers** — monitor project memberships and high-level story distribution through simple queries.




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pivotal Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active stories in project 12345."

**🤖 AI Agent:**
> I've retrieved 8 active stories from project 12345. Current ones include 'Implement OAuth2 flow', 'Fix CSS bug in dashboard', and 'Add user profile export'.

---

**👤 You:**
> "Create a new bug story in project 12345 called 'Broken login button'."

**🤖 AI Agent:**
> Bug story 'Broken login button' has been successfully created in project 12345. Story ID: 987654321.

---

**👤 You:**
> "Update story 987654321 to 'started' state."

**🤖 AI Agent:**
> Story 987654321 has been updated to 'started'. You can now begin work on this task.


## ❓ FAQ

**Q: How do I find my Pivotal Tracker API Token?**
Log in to Pivotal Tracker, click on your name in the top right, go to **Profile Settings**, and scroll down to the **API Token** section.

**Q: Can I filter stories by their current state?**
Yes! Use the `list_stories` tool and provide a filter like `state:started` or `state:unscheduled` to narrow down the results.

**Q: Does this support checking project memberships?**
Absolutely. Use the `list_memberships` tool with a Project ID to see all users associated with that specific project and their roles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pivotal-tracker](https://vinkius.com/mcp/pivotal-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pivotal Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pivotal-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pivotal Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pivotal-tracker": {
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
