# Lancerkit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lancerkit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [crm-sales](../categories/crm-sales.md)

Connect Lancerkit to any AI agent via MCP.



## Available Tools (10)
- **get_client**: Retrieve specific metadata of one single client
- **get_invoice**: Retrieve data, payments, and billings for a specific invoice string ID
- **get_project**: Get a single project details by ID
- **get_status**: Examine account and integration connection status overall
- **get_time_logs**: Check the recorded time logs for hours spent
- **list_clients**: List all clients associated with the workspace
- **list_invoices**: Fetch global invoice pipeline statistics
- **list_projects**: List all standard projects
- **list_services**: Fetch all specific billable service items configured online
- **list_tasks**: Check current working tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lancerkit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Draft an invoice for the Acme Corp redesign project."

**🤖 AI Agent:**
> I have drafted an invoice for Acme Corp. The invoice includes 40 hours of UI/UX design at $75/hr and a fixed fee of $1,000 for the logo, totaling $4,000. Would you like me to send it?

---

**👤 You:**
> "How many billable hours have I tracked this week?"

**🤖 AI Agent:**
> You have tracked 28 billable hours this week across 3 clients. The breakdown is: 15 hours for Delta Tech, 8 hours for Acme Corp, and 5 hours for Omega Inc.

---

**👤 You:**
> "Create a new project named Mobile App Development for Delta Tech."

**🤖 AI Agent:**
> I have successfully created the new project 'Mobile App Development' and assigned it to the client Delta Tech. I've also set up the default hourly rate of $85/hr for this project.


## ❓ FAQ

**Q: What is Lancerkit?**
Lancerkit is an all-in-one platform for freelancers to manage projects, track time, send invoices, and handle client communication from a single dashboard.

**Q: Where do I find my API key?**
You can find your API key in the Lancerkit dashboard under Account Settings > Developer API. Generate a new token with appropriate permissions.

**Q: Can I create invoices automatically using natural language?**
Yes, you can instruct the AI to draft, review, and send invoices to your clients based on your tracked time or fixed project milestones.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lancerkit](https://vinkius.com/mcp/lancerkit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lancerkit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lancerkit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lancerkit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lancerkit": {
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
