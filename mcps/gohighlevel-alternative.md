# GoHighLevel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gohighlevel-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage your GHL location — audit contacts, opportunities, and tasks via AI.

## Description
Empower your AI agent to orchestrate your entire marketing and sales ecosystem with **GoHighLevel** (GHL), the all-in-one sales and marketing platform. By connecting GHL to your agent, you transform complex CRM management into a natural conversation. Your agent can instantly list your contacts, audit sales opportunities, and manage daily tasks without you ever touching a dashboard. Whether you are running a small business or a large agency, your agent acts as a real-time CRM operator, ensuring your leads are always nurtured and your pipeline is healthy.

### What you can do

- **Contact Management** — List, retrieve, create, and update contact profiles to maintain a deep understanding of your audience.
- **Opportunity Oversight** — Query pipelines and audit specific sales opportunities to stay on top of your revenue funnel.
- **Task & Appointment Tracking** — Monitor daily tasks and upcoming appointments to ensure no lead is forgotten.
- **User Administration** — List all users in the location to maintain organizational control and audit access.
- **Location Auditing** — Quickly retrieve location-wide metadata to understand your account status in real-time.

### How it works

1. Subscribe to this server
2. Enter your GHL Location API Key
3. Start managing your CRM data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Managers** — monitor lead flow and opportunity statuses straight from your workflow.
- **Account Executives** — verify if new contacts have been correctly created and assigned to pipelines.
- **Marketing Leads** — perform rapid audits of contact lists and check task completion without manual dashboard logins.
- **Agency Owners** — automate CRM querying to orchestrate cross-functional client teams smoothly.




## 💬 Prompt Examples

Here are some examples of how you can interact with the **GoHighLevel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 contacts added to GHL."

**🤖 AI Agent:**
> I've retrieved your recent contacts. You have 5 new entries, including 'John Doe' and 'Jane Smith'. Would you like the full details for any of them?

---

**👤 You:**
> "Show me my open sales opportunities."

**🤖 AI Agent:**
> I've found 3 open opportunities in your pipeline: 'New Software Deal', 'Consulting Package', and 'Q4 License'. I can provide the estimated value for each if you like.

---

**👤 You:**
> "What tasks are assigned to contact ID 12345?"

**🤖 AI Agent:**
> Checking tasks for that contact... I've found 2 pending tasks: 'Follow up call' and 'Send proposal'. Both are currently due this week.


## ❓ FAQ

**Q: How do I find my GHL Location API Key?**
Log in to your GHL account, go to **Settings** > **Business Profile**, and you will find your API Key under the **General** section. Copy and paste it into the field below.

**Q: Can the agent list all opportunities in my pipeline?**
Yes. Use the `list_opportunities` tool to retrieve all sales opportunities across your pipelines. Your agent will present them with their current status and value.

**Q: Is it possible to update contact details via the agent?**
Yes. The `update_contact` tool allows your agent to modify existing contact information, such as email or names, by providing the specific Contact ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gohighlevel-alternative](https://vinkius.com/mcp/gohighlevel-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GoHighLevel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gohighlevel-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GoHighLevel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gohighlevel-alternative": {
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
