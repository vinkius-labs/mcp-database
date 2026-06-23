# Tally MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tally)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Tally forms and submissions — audit workspaces and responses via AI.

## Description
Empower your AI agent to orchestrate your entire form ecosystem with **Tally**, the simplest way to create forms. By connecting Tally to your agent, you transform complex submission management into a natural conversation. Your agent can instantly list your forms, audit new submissions, and retrieve workspace details without you ever touching a dashboard. Whether you are running a simple survey or a complex lead generation process, your agent acts as a real-time form manager, ensuring your data is always accessible and organized.

### What you can do

- **Form Auditing** — List all forms in your account and retrieve detailed metadata for each, including workspace associations.
- **Submission Management** — Query new and historical submissions, and retrieve specific entry details instantly.
- **Workspace Oversight** — List all your Tally workspaces and monitor form distribution across your organization.
- **Data Governance** — Autonomously delete submissions when they are no longer needed to maintain data privacy.
- **Account Auditing** — Quickly retrieve account-wide information to maintain strict organizational control.

### How it works

1. Subscribe to this server
2. Enter your Tally API Key
3. Start managing your forms and data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — monitor user feedback and survey results straight from your workflow.
- **Operations Leads** — verify if new submissions are being correctly captured and processed by the team.
- **Support Teams** — perform rapid submission audits and verify user inputs without manual dashboard logins.
- **Business Owners** — automate data querying to orchestrate your form-driven growth smoothly.


## Available Tools (8)
- **delete_submission**: Delete a Tally submission
- **get_form**: Get details for a specific form
- **get_me**: Get Tally account details
- **get_submission**: Get details for a specific submission
- **get_workspace**: Get details for a specific workspace
- **list_forms**: Optional: filter by workspace ID.

List Tally forms
- **list_submissions**: List submissions for a Tally form
- **list_workspaces**: List all Tally workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tally** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Tally forms."

**🤖 AI Agent:**
> I've retrieved your forms. You have 4 active forms, including 'User Feedback' and 'Lead Gen 2024'. Would you like to see the submissions for any of them?

---

**👤 You:**
> "Show me the last 5 submissions for form ID 12345."

**🤖 AI Agent:**
> I've found the last 5 submissions for that form. They include responses from 'john@doe.com' and 4 others. Would you like the full details for the most recent one?

---

**👤 You:**
> "What workspaces do I have in Tally?"

**🤖 AI Agent:**
> You have 2 workspaces: 'Personal' and 'Marketing Team'. I can list the forms associated with either workspace if you like.


## ❓ FAQ

**Q: How do I find my Tally API Key?**
Log in to your Tally account, go to **Settings** > **API**, and you will find your API Key there. Copy and paste it into the field below.

**Q: Can the agent list submissions for a specific form?**
Yes. Use the `list_submissions` tool by providing the Form ID. Your agent will retrieve all entries and present them in a structured format.

**Q: Is it possible to manage multiple workspaces?**
Yes. The `list_workspaces` tool allows you to see all workspaces you have access to, and you can filter forms by `workspaceId`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tally](https://vinkius.com/mcp/tally)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tally** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tally` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tally** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tally": {
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
