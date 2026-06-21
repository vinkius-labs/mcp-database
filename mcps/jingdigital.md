# JingDigital MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jingdigital)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Marketing automation platform for the WeChat ecosystem — manage contacts, campaigns, and stats via AI.

## Description
Empower your AI agent to orchestrate your marketing operations within the WeChat ecosystem with **JingDigital**, the leading customer engagement platform for China. By connecting JingDigital to your agent, you transform complex customer segmentation, campaign tracking, and WeChat workflow management into a natural conversation. Your agent can instantly list CRM contacts, retrieve detailed profile information, monitor marketing campaigns, and even provide account-wide statistics without you ever needing to navigate the comprehensive web interface. Whether you are managing high-volume customer inquiries or complex automation flows, your agent acts as a real-time marketing assistant, keeping your data accurate and your engagement moving.

### What you can do

- **Contact Orchestration** — List and retrieve detailed information about your CRM contacts and followers.
- **Campaign Management** — Browse active marketing campaigns and retrieve detailed performance metadata.
- **Workflow Monitoring** — List and audit automation workflows to ensure your marketing logic is operating correctly.
- **Asset Control** — Browse your digital asset library and identify resources for use in your campaigns.
- **Performance Insights** — Retrieve high-level statistics on account performance and engagement levels.

### How it works

1. Subscribe to this server
2. Enter your JingDigital App ID and App Secret
3. Start managing your WeChat marketing through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — monitor campaign progress and audit customer segments through natural language queries.
- **Customer Success Teams** — manage CRM contacts and retrieve detailed interaction histories directly from your AI-powered workspace.
- **Operations Leads** — oversee automation workflows and account statistics via a unified AI interface.
- **WeChat Power Users** — integrate your existing JingDigital workflows into your AI-driven daily routines.


## Available Tools (10)
- **create_contact**: Create a new contact
- **get_account_info**: Get account metadata
- **get_campaign**: Get campaign details
- **get_contact**: Get contact details
- **get_stats**: Get account statistics
- **list_assets**: ) in the library.

List marketing assets
- **list_campaigns**: List marketing campaigns
- **list_contacts**: List CRM contacts
- **list_events**: List tracking events
- **list_workflows**: List automation workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JingDigital** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all CRM contacts from JingDigital."

**🤖 AI Agent:**
> I've retrieved your CRM contacts. You have 1,200 total followers, including 50 high-value leads marked with specific segmentation tags. Would you like to view the details of the most active ones?

---

**👤 You:**
> "Show me the performance stats for the last 30 days."

**🤖 AI Agent:**
> I've listed the account statistics for the last 30 days. You've gained 450 new followers and reached a 15% conversion rate across your active campaigns. Should I break this down by specific marketing touchpoints?

---

**👤 You:**
> "Check the status of campaign 'Summer-Promo-2026'."

**🤖 AI Agent:**
> The 'Summer-Promo-2026' campaign is currently active. It has been sent to 5,000 recipients with an open rate of 42%. Would you like to see the breakdown of engagement per workflow step?


## ❓ FAQ

**Q: How do I find my JingDigital App ID and Secret?**
Log in to your JingDigital administration portal, navigate to the [Developer Center] or [Application Management] section, and you will find your unique App ID and App Secret for API access.

**Q: Can I see interaction histories through this server?**
Yes. Use the `list_events` tool to retrieve historical behavioral and tracking data for your contacts. This is essential for auditing engagement and understanding the customer journey.

**Q: Is it possible to monitor automation workflows?**
Yes! You can use the `list_workflows` tool to see all your marketing automation flows and identify which ones are currently active or pending.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jingdigital](https://vinkius.com/mcp/jingdigital)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JingDigital** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jingdigital` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JingDigital** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jingdigital": {
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
