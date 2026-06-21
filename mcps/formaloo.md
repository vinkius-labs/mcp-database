# Formaloo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/formaloo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Automate data collection and management via Formaloo — search boards, list assigned rows, and manage form blueprints directly from any AI agent.

## Description
Connect your **Formaloo** account to any AI agent to streamline your data collection, form management, and database workflows through natural conversation.

### What you can do

- **Board Management** — Search, list, create, and update boards or folders to organize your data structures efficiently.
- **Data Inspection** — Retrieve assigned rows and form submissions with advanced filtering by tags, tracking codes, or dates.
- **Blueprints & Templates** — Access detailed blueprints to understand form structures and replicate successful data models.
- **Infrastructure Control** — Manage available email servers and business addon packages to power your automation.
- **API Management** — Request and refresh API keys directly through the agent for secure application development.

### How it works

1. Subscribe to this server
2. Enter your Formaloo API Key (and optional JWT/Workspace ID)
3. Start managing your databases and forms from Claude, Cursor, or any MCP-compatible client

Your AI acts as a data architect, helping you query submissions and organize boards without manual dashboard navigation.

### Who is this for?

- **Data Analysts** — quickly query form submissions and assigned rows to generate insights without exporting CSVs.
- **Operations Managers** — organize boards and folders to keep company data structures clean and accessible.
- **Developers** — manage API keys and inspect blueprint metadata directly from the coding environment.


## Available Tools (14)
- **list_access_type_descriptions**: Get Access Type Description List
- **list_active_packages**: Get Business Addon Packages List
- **list_addons**: Get Addon List
- **list_assigned_rows**: Get Assigned Rows List
- **list_available_email_servers**: Get Email Server Available List
- **get_blueprint**: Blue Print Detail
- **copy_board**: Board Copy
- **create_available_email_server**: Create Email Server Available
- **create_board**: Create User Board
- **get_board**: Board Detail
- **list_boards**: Get User Board List
- **request_api_key**: Request Api Key
- **search_boards**: Search Boards And Folders
- **update_board**: Update Board


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Formaloo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all boards related to 'Customer Feedback'."

**🤖 AI Agent:**
> I found 3 boards matching 'Customer Feedback': 'Q1 Survey' (Slug: q1-survey), 'Product Reviews' (Slug: product-reviews), and 'Support Tickets' (Slug: support-tickets).

---

**👤 You:**
> "List the rows assigned to my forms that were created this week."

**🤖 AI Agent:**
> I've retrieved the assigned rows for this week. There are 12 new entries across your active forms. Would you like me to summarize the data from the 'Contact Us' form?

---

**👤 You:**
> "Get the details of the blueprint with slug 'event-registration'."

**🤖 AI Agent:**
> Inspecting blueprint 'event-registration'... This template includes fields for Name, Email, Ticket Type, and Dietary Requirements. It is currently used in 2 of your active boards.


## ❓ FAQ

**Q: How can I find a specific board or folder by name?**
You can use the `search_boards` tool. Simply provide a search term, and the agent will return all matching boards and folders from your Formaloo account.

**Q: Can I view the data submitted to my forms through the AI?**
Yes! Use the `list_assigned_rows` tool. You can filter the results by form, tags, creator, or date to find exactly the submissions you need.

**Q: Is it possible to see the structure of a form template?**
Absolutely. Use the `get_blueprint` tool with the specific blueprint slug to retrieve its full technical details and structure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/formaloo](https://vinkius.com/mcp/formaloo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Formaloo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `formaloo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Formaloo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "formaloo": {
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
