# ClickFunnels MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clickfunnels)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage sales funnels and contacts via ClickFunnels 2.0 — track performance, monitor leads, and manage orders directly from any AI agent.

## Description
Connect your **ClickFunnels 2.0** account to any AI agent and take full control of your sales funnels and marketing automation through natural conversation. Streamline how you monitor your business growth natively.

### What you can do

- **Funnel Oversight** — List and retrieve details for all sales funnels and their constituent steps natively
- **Contact Intelligence** — Access and monitor all identified contacts and leads within your workspaces flawlessly
- **Team & Workspace Management** — List all teams and workspaces associated with your account securely
- **Order Tracking** — Access and review customer orders and transactional history flawlessly
- **Product Logistics** — List products and offers available in your funnels flawlessly
- **Growth Visibility** — Retrieve detailed funnel metadata and performance metrics directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your ClickFunnels 2.0 Access Token and Subdomain
3. Start managing your marketing funnels from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Digital Marketers** — monitor funnel conversion rates and lead volume using natural language
- **E-commerce Owners** — review recent orders and product performance without opening the dashboard
- **Sales Teams** — quickly look up contact profiles and engagement history straight from their chat interface
- **Marketing Ops** — verify funnel structure and automated steps


## Available Tools
- **list_funnels**: List funnels
- **list_contacts**: List contacts
- **get_contact**: Get contact
- **create_contact**: Create contact
- **list_orders**: List orders
- **get_order**: Get order
- **list_workflows**: List workflows
- **list_tags**: List tags


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ClickFunnels** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my sales funnels in workspace 'ws_12345'."

**🤖 AI Agent:**
> Retrieving your funnels... I found 4 items: 'High-Ticket Coaching', 'E-book Lead Magnet', 'Webinar Series', and 'Order Confirmation'. Which one would you like to see the steps for?

---

**👤 You:**
> "Show me the last 5 orders from my 'E-book' funnel."

**🤖 AI Agent:**
> Checking recent orders... I found 5 sales for the 'E-book' funnel today. All are marked as 'Completed' and processed successfully. Total revenue from these is $485.00.

---

**👤 You:**
> "Who are the newest leads in my workspace?"

**🤖 AI Agent:**
> Retrieving newest contacts... The 3 latest leads are: Sarah Smith (sarah@example.com), Mike Miller (mike@gmail.com), and Jane Doe (jane@outlook.com). All joined within the last 2 hours.


## ❓ FAQ

**Q: Can I see the steps inside a specific funnel?**
Yes! Use the `list_funnel_steps` tool with the funnel ID. The agent will return all pages and actions configured within that funnel.

**Q: How do I find a contact by their email address?**
Use the `list_funnel_contacts` tool. While it lists contacts in a workspace, you can ask the agent to find a specific person by email within that list.

**Q: Where do I find my ClickFunnels 2.0 Access Token?**
Log in to your ClickFunnels 2.0 dashboard, go to **Settings**, and select **API**. You can create and copy your access token from that section.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clickfunnels](https://vinkius.com/mcp/clickfunnels)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ClickFunnels** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `clickfunnels` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ClickFunnels** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clickfunnels": {
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
