# Smaily MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/smaily)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate email marketing and automations via Smaily — manage subscribers, campaigns, and responders directly from any AI agent.

## Description
Connect your **Smaily** account to any AI agent and simplify your email marketing and automation workflows through natural conversation.

### What you can do

- **Subscriber Management** — List all contacts in your database, retrieve detailed profile metadata, and create new subscribers programmatically
- **Campaign Control** — Query past and scheduled email campaigns to monitor your marketing outreach
- **Automation & Autoresponders** — List configured automated workflows and trigger specific autoresponder emails directly from your agent
- **Template catalog** — Query available email templates to choose the right look for your messages
- **Operational tracking** — Stay on top of your marketing performance and subscriber engagement

### How it works

1. Subscribe to this server
2. Enter your Smaily Subdomain, API User, and API Password from your account settings
3. Start managing your email marketing from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **delete_subscriber**: Remove a subscriber
- **get_automation**: Get details for an automation workflow
- **get_campaign**: Get details for a specific campaign
- **get_template**: Get details for an email template
- **create_subscriber**: Add a new subscriber
- **get_subscriber_details**: Get details for a specific subscriber
- **list_automations**: List automated responders
- **list_email_campaigns**: List email campaigns
- **list_subscribers**: List Smaily subscribers
- **list_email_templates**: List message templates
- **send_automation_email**: Trigger an automation email


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Smaily** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all subscribers in Smaily."

**🤖 AI Agent:**
> I've retrieved your contact list. You have 500 subscribers, including 'john@example.com' and 'alice@smith.co'.

---

**👤 You:**
> "Show me the campaign performance for all email campaigns sent this quarter with engagement trends."

**🤖 AI Agent:**
> 18 campaigns sent this quarter. Total sent: 67,800. Overall open rate: 32.4% (up from 28.1% last quarter). Click rate: 5.8% (+0.9%). Unsubscribe rate: 0.14%. Top performer: "Spring Collection Launch" (45.2% open, 9.8% click). Lowest: "Monthly Digest #3" (18.4% open). A/B test insights: personalized subjects outperform generic by 34%. Best send time: Tuesday 10 AM. Automation emails (6 workflows): 89,000 sent, 42% open rate. List growth: +1,234 net subscribers.

---

**👤 You:**
> "Create a new subscriber and add them to the VIP customer automation workflow."

**🤖 AI Agent:**
> Subscriber created: Maria Santos (maria@meridian.io). Tags: VIP, Enterprise, Q2-2025. Custom fields: Company (Meridian Corp), Role (VP Marketing), Source (Referral). Added to automation: "VIP Customer Journey". Workflow steps: Day 0 - Welcome email (personalized). Day 3 - Exclusive preview of new features. Day 7 - Personal thank you from CEO. Day 14 - Quarterly review invitation. Day 30 - Loyalty reward notification. Subscriber status: Active. GDPR consent: recorded.


## ❓ FAQ

**Q: Can I list all my email templates using my AI agent?**
Yes! Use the `list_email_templates` tool to retrieve a comprehensive list of all message templates available in your Smaily account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smaily](https://vinkius.com/mcp/smaily)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Smaily** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `smaily` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Smaily** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "smaily": {
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
