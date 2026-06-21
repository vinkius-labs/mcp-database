# Attio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/attio-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Build powerful CRM workflows with flexible data models, relationship tracking, and deal management tailored to your process.

## Description
Connect your **Attio** account to any AI agent and take full control of your relationship management orchestration and automated CRM workflows through natural conversation.

### What you can do

- **Object & Record Orchestration** — List and manage your entire database of CRM objects (Companies, People) programmatically, retrieving detailed attribute metadata
- **Relationship Intelligence Architecture** — Programmatically query and monitor customer interactions and connection signals to maintain a perfectly coordinated sales strategy
- **Workflow & View Monitoring** — Access your complete directory of CRM views and pipelines to coordinate your organizational resource allocation in real-time
- **Metadata Management** — Programmatically retrieve field identifiers and record history to maintain a perfectly coordinated audit trail
- **Operational Monitoring** — Verify account-level API connectivity and monitor CRM activity volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Attio dashboard (Settings > API Keys)
3. Start orchestrating your business growth from Claude, Cursor, or any MCP client

No more manual updating of individual CRM records or missing critical relationship updates. Your AI acts as your dedicated relationship coordinator and CRM architect.

### Who is this for?

- **Sales & Success Managers** — instantly retrieve relationship summaries and monitor pipeline health using natural language commands
- **Operations Leads** — verify individual record metadata and track CRM updates without leaving your creative workspace
- **Developers** — integrate high-speed Attio data into custom internal tools and communication channels through simple AI queries


## Available Tools
- **check_attio_status**: Verify Attio API connectivity
- **create_note**: Useful for logging meeting notes, call summaries, or updates.

Create a note on a record
- **create_record**: Pass attribute values as JSON (e.g., {"name": [{"value": "Acme Corp"}]}).

Create a new record
- **create_task**: Create a new task
- **delete_record**: This action is irreversible.

Delete a record
- **get_list_entries**: Get entries from a list
- **get_object**: Get object schema
- **get_record**: Get a specific record
- **list_lists**: List all lists
- **list_notes**: List notes on a record
- **list_objects**: List all CRM objects
- **list_records**: Use "companies" for companies, "people" for contacts, "deals" for deals.

List records for any object
- **list_tasks**: List all tasks
- **update_record**: Only provided attributes are changed.

Update an existing record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Attio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all records in the 'Companies' object in my Attio account and show the last 5 entries."

**🤖 AI Agent:**
> I've retrieved your company records. You currently have 100 companies. The last 5 entries include 'Global Corp' and 'Startup X'. Would you like the detailed attribute metadata for any of them?

---

**👤 You:**
> "Show the recent updates for 'John Doe' in the 'People' object."

**🤖 AI Agent:**
> Relationship intelligence orchestrated! For John Doe, I've identified the last 3 updates, including a job title change and a new interaction log at 2:00 PM today. I've retrieved the technical attribute metadata for your review. Need help notifying the success team?

---

**👤 You:**
> "Check for any active pipelines with zero updates this week."

**🤖 AI Agent:**
> Operational monitoring orchestrated! I've identified 2 pipelines with zero activity this week, including 'Partnership Beta' and 'Outreach Alpha'. I've retrieved the technical status for your review. Shall I check for any pending record updates in these pipelines?


## ❓ FAQ

**Q: How do I find my Attio API Key?**
Log in to your account, navigate to **Settings** > **API Keys**, and create or copy your unique Access Token.

**Q: Can I retrieve records from a specific object via AI?**
Yes! The `list_records` tool allows your agent to retrieve metadata for all entries in a specific CRM object (e.g., 'people' or 'companies').

**Q: How do I list my active CRM objects?**
Use the `list_objects` tool to retrieve your complete directory along with the unique identifiers for all managed CRM schemas.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/attio-alternative](https://vinkius.com/mcp/attio-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Attio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `attio-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Attio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "attio-alternative": {
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
