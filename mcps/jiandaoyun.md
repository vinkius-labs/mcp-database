# Jiandaoyun MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jiandaoyun)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Cloud-based zero-code data management platform — manage forms, records, and workflows via AI.

## Description
Empower your AI agent to orchestrate your data workflows with **Jiandaoyun**, the leading zero-code platform for enterprise applications. By connecting Jiandaoyun to your agent, you transform complex form management and data entry into a natural conversation. Your agent can instantly list your applications, retrieve form schemas, create or update records, and even check workflow statuses without you needing to navigate the web interface. Whether you are managing inventory, HR records, or customer data, your agent acts as a real-time data assistant, keeping your records accurate and your processes moving.

### What you can do

- **Application Management** — List all accessible applications and browse the forms within them.
- **Form Operations** — Retrieve field schemas and manage data records (create, list, update, delete) with ease.
- **Workflow Tracking** — Monitor the current status of workflows for specific form records.
- **Data Insights** — Retrieve detailed record information for analysis and decision-making.
- **Team Coordination** — Access the organization's address book to manage user-related data.

### How it works

1. Subscribe to this server
2. Enter your Jiandaoyun API Key
3. Start managing your data and forms through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — automate data collection and monitor business processes through natural language.
- **Data Analysts** — retrieve and audit form records directly from your AI-powered workspace.
- **HR & Admin Teams** — manage employee records and internal requests through a unified AI interface.
- **Small Business Owners** — oversee inventory and customer tracking without complex technical overhead.


## Available Tools (10)
- **create_record**: Create a new form record
- **delete_record**: Delete a form record
- **get_form_schema**: Get form field schema
- **get_record_details**: Get record details
- **get_workflow_status**: Get record workflow status
- **list_address_book**: List organization users
- **list_apps**: List all Jiandaoyun applications
- **list_data**: List records in a form
- **list_forms**: List forms in an application
- **update_record**: Update an existing form record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jiandaoyun** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all forms in the 'Sales Pipeline' application."

**🤖 AI Agent:**
> I've retrieved the forms for 'Sales Pipeline'. You have 3 forms: 'Leads', 'Opportunities', and 'Contracts'. Which one would you like to view data for?

---

**👤 You:**
> "Show me the last 5 records from the 'Inventory' form."

**🤖 AI Agent:**
> I've listed the last 5 records from 'Inventory'. Items include 'Laptop Model X' and 'Office Chair Z'. Would you like to see the details of any specific item?

---

**👤 You:**
> "What is the workflow status for record ID 'rec-12345' in the 'Expense Reimbursement' form?"

**🤖 AI Agent:**
> The record 'rec-12345' is currently at the 'Manager Approval' step. The status is 'In Progress'. Would you like me to notify the current assignee?


## ❓ FAQ

**Q: How do I find my Jiandaoyun API Key?**
Log in to Jiandaoyun, go to [Account Center] → [Account Settings] → [API Key], and generate your token there. Ensure your version supports API access.

**Q: Can I check the status of an approval process?**
Yes. Using the `get_workflow_status` tool with the application, form, and record IDs, you can retrieve the current step and status of any active workflow/approval process.

**Q: How do I know which fields to use when creating a record?**
Use the `get_form_schema` tool. it will return all the available widgets (fields) for that form, including their unique IDs which you need to use in the `data` parameter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jiandaoyun](https://vinkius.com/mcp/jiandaoyun)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jiandaoyun** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jiandaoyun` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jiandaoyun** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jiandaoyun": {
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
