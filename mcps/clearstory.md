# Clearstory MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clearstory)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage construction change orders and T&M tags via Clearstory — track projects, monitor CORs, and manage project rates directly from any AI agent.

## Description
Connect your **Clearstory** account to any AI agent and take full control of your construction project financial data through natural conversation. Streamline how you manage Change Order Requests (CORs) and Time & Material (T&M) tags natively.

### What you can do

- **Project Oversight** — List and retrieve details for all active and inactive construction projects natively
- **COR Intelligence** — Access and monitor Change Order Requests, including amounts and statuses flawlessly
- **Tag Management** — List and review digital Time & Material tags directly from the field securely
- **Contract Auditing** — Access contracts linked to specific change orders flawlessly
- **Notification Logistics** — List and review change notifications sent between customers and contractors flawlessly
- **Rate Visibility** — Monitor Labor, Material, Equipment, and Other (LMEO) rates for your projects directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Clearstory API Key (obtained from Settings > Offices > Integrations)
3. Start managing your construction financial data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — monitor COR statuses and project health using natural language
- **Specialty Contractors** — review T&M tags and change notifications without opening the dashboard
- **Finance Teams** — quickly look up contract details and project rates straight from their chat interface
- **General Contractors** — verify change order volumes and supply chain risk across projects


## Available Tools
- **get_cor_details**: Get detailed information for a specific COR
- **get_project_construction_details**: Get detailed information for a specific project
- **list_change_order_requests**: List all Change Order Requests (CORs)
- **list_project_contracts**: List contracts linked to change orders
- **list_change_notifications**: List change notifications sent between customers and contractors
- **list_construction_projects**: List all construction projects in Clearstory
- **list_construction_rates**: List Labor, Material, Equipment, and Other (LMEO) rates
- **list_tm_tags**: List digital Time & Material tags from the field


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clearstory** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active construction projects in Clearstory."

**🤖 AI Agent:**
> Retrieving your active projects... I found 4 projects: 'City Hospital Expansion', 'Eastside Towers', 'Green Street Plaza', and 'Downtown Refurb'. Which one would you like to see CORs for?

---

**👤 You:**
> "Show me the last 5 Change Order Requests."

**🤖 AI Agent:**
> Checking recent CORs... I found 5 items ranging from $500 to $12,000. The most recent is COR #105 for 'Additional Electrical Outlets' ($1,250) in status 'Pending'.

---

**👤 You:**
> "What are the labor rates for the 'City Hospital' project?"

**🤖 AI Agent:**
> Retrieving rates for City Hospital... The standard labor rate is $85/hr for Journeymen and $65/hr for Apprentices. These are configured under the project's LMEO settings.


## ❓ FAQ

**Q: Can I see the total amount of outstanding CORs for a project?**
Yes! Use the `list_change_order_requests` tool. The agent will return all CORs, and you can ask it to calculate or filter for the total value of those in 'Pending' or 'Under Review' status.

**Q: How do I check the latest T&M tags from the field through the agent?**
Use the `list_tm_tags` tool. Your agent will fetch the most recent digital Time & Material tags, allowing you to review labor hours and material usage without opening the web app.

**Q: Where do I find my Clearstory API Key?**
Log in to Clearstory, navigate to **Settings > Offices**, select your office, and go to the **Integrations** tab. You can generate and copy your API key from there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clearstory](https://vinkius.com/mcp/clearstory)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clearstory** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `clearstory` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clearstory** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clearstory": {
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
