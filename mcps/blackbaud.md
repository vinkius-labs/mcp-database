# Blackbaud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blackbaud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Manage constituents, gifts, and academic data via Blackbaud — handle fundraising and education management directly from your AI agent.

## Description
Connect your **Blackbaud** account to any AI agent to streamline nonprofit fundraising and education management through natural conversation.

### What you can do

- **Constituent Management** — Create, retrieve, and update constituent records to keep your donor database current.
- **Gift Tracking** — Record new donations and fetch detailed gift information to monitor fundraising progress.
- **Education Management** — List school users (students, faculty) and retrieve academic section information for institutional oversight.
- **Data Updates** — Modify existing constituent details directly through the agent to ensure data integrity.

### How it works

1. Subscribe to this server
2. Enter your Blackbaud Access Token and Subscription Key
3. Start managing your nonprofit or educational data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Nonprofit Managers** — quickly check donor history and record new gifts without navigating complex CRM menus.
- **School Administrators** — access student and faculty lists and academic sections directly from their workflow.
- **Development Officers** — update constituent information on the fly during donor outreach.


## Available Tools (7)
- **create_constituent**: Create a new constituent
- **create_gift**: Record a new gift
- **get_constituent**: Retrieve a constituent record
- **get_gift**: Retrieve gift details
- **list_academic_sections**: Retrieve academic section information
- **list_school_users**: ) within Blackbaud education management.

List school users
- **update_constituent**: Update constituent details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blackbaud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve the constituent record for ID 54321."

**🤖 AI Agent:**
> I've retrieved the record for constituent 54321. It belongs to 'Sarah Jenkins', classified as an 'Individual' donor. Would you like to see her recent gift history?

---

**👤 You:**
> "Record a gift of 250.00 for constituent 10101 dated 2023-11-15."

**🤖 AI Agent:**
> Successfully recorded the gift! A donation of $250.00 has been added to constituent 10101's record for November 15, 2023.

---

**👤 You:**
> "List all current academic sections."

**🤖 AI Agent:**
> I've fetched the academic sections. There are currently 12 active sections, including 'Advanced Mathematics - Section A' and 'Intro to Biology'. Do you need details on a specific one?


## ❓ FAQ

**Q: How can I find the specific details of a donor using their ID?**
You can use the `get_constituent` tool. Simply provide the Constituent ID, and the agent will retrieve their full record, including names and types.

**Q: Is it possible to record a new donation directly through the AI?**
Yes! Use the `create_gift` tool by providing the constituent ID, the amount, and the date. The agent will record the donation in Blackbaud for you.

**Q: Can I see a list of students or faculty members in the system?**
Certainly. The `list_school_users` tool retrieves a list of users within the Blackbaud education management system, including students and faculty.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blackbaud](https://vinkius.com/mcp/blackbaud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blackbaud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `blackbaud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blackbaud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blackbaud": {
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
