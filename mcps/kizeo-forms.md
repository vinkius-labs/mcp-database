# Kizeo Forms MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kizeo-forms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage mobile forms, data submissions, and users via the Kizeo Forms API.

## Description
Connect your **Kizeo Forms** account to any AI agent to automate your field data collection and operational workflows. This MCP server enables your agent to interact with mobile forms, manage data submissions, and query user permissions directly from natural language interfaces.

### What you can do

- **Form Oversight** — List all available mobile forms and retrieve their hierarchical structures and field definitions
- **Data Management** — Retrieve specific form entries and perform advanced searches using custom field filters
- **Push Operations** — Pre-fill and push new data entries into forms to streamline field work assignments
- **User Administration** — Manage account users, update profiles, and control permissions across your organization
- **Operational Auditing** — Read unread data submissions and monitor field activity in real-time

### How it works

1. Subscribe to this server
2. Enter your Kizeo Forms Authorization Token
3. Start managing your mobile forms from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — Monitor field data submissions and assign tasks via natural language commands
- **Field Supervisors** — Quickly query form definitions and entry data without opening the web interface
- **Developers** — Integrate mobile form logic and data pushing into your custom operational tools


## Available Tools (9)
- **create_new_user**: Requires name, email, and password.

Add a new user to the account
- **delete_account_user**: Remove a user from the account
- **list_all_forms**: List all available forms
- **search_form_data**: Search form data with advanced filters
- **get_form_entry_data**: Get data for a specific form submission
- **get_form_definition**: Get the definition of a specific form
- **push_data_to_form**: Requires a JSON body with field values.

Push a new data entry into a form
- **update_existing_user**: Update details for an existing user
- **list_account_users**: List all users in the account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kizeo Forms** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my available forms in Kizeo."

**🤖 AI Agent:**
> I've retrieved your forms. You have 5 active forms, including 'Inspection Report' (ID: 12345), 'Time Tracking' (ID: 67890), and 'Inventory Audit' (ID: 11223).

---

**👤 You:**
> "Search for submissions in form ID '12345' where status is 'Pending'."

**🤖 AI Agent:**
> I found 3 submissions in form 12345 matching your criteria. Recent entries include data from 'Site A' and 'Site B'. Would you like to see the full details for any of them?

---

**👤 You:**
> "Push a new entry to form '67890' with technician name 'Jane Doe' and site 'South Station'."

**🤖 AI Agent:**
> Successfully pushed the new entry to form 67890. The data has been recorded and is now available for the technician in the field.


## ❓ FAQ

**Q: How do I find my Form ID?**
Use the `list_all_forms` tool to see a comprehensive list of all forms in your account along with their unique IDs.

**Q: Can I filter form data using specific fields?**
Yes, the `search_form_data` tool allows you to perform advanced searches by providing a JSON object with your filtering criteria.

**Q: Is it possible to push data to a form via the agent?**
Absolutely. Use the `push_data_to_form` tool with the target Form ID and a JSON object containing the field values you want to pre-fill.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kizeo-forms](https://vinkius.com/mcp/kizeo-forms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kizeo Forms** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kizeo-forms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kizeo Forms** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kizeo-forms": {
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
