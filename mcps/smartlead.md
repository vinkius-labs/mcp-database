# SmartLead MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/smartlead)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent with direct access to SmartLead — manage cold email campaigns, rotate sending accounts, and scale outreach without opening the SmartLead dashboard.

## Description
Connect **SmartLead** to your AI agent and manage your cold email infrastructure at scale.

### What you can do

- **Campaign Management** — Create, edit, and monitor campaigns with multi-mailbox rotation.
- **Lead Management** — Upload leads, track statuses, and manage engagement across campaigns.
- **Email Account Rotation** — Monitor sending accounts, warm-up scores, and inbox placement rates.
- **Analytics** — Pull campaign performance metrics including opens, clicks, replies, and conversions.

### How it works

1. Subscribe to the SmartLead integration on the marketplace.
2. Get your API key from your SmartLead dashboard (Settings → API → copy the key).
3. Ask your AI agent to manage campaigns, check deliverability, or track leads.

### Who is this for?

- **Cold Email Agencies** — Scale outreach across hundreds of mailboxes and client campaigns.
- **SDR Teams** — Run high-volume campaigns with built-in mailbox rotation and warm-up.
- **Lead Gen Companies** — Automate prospect engagement at industrial scale.


## Available Tools (8)
- **get_campaign**: Get campaign
- **get_campaign_analytics**: Get campaign analytics
- **list_leads**: List leads
- **add_lead**: Add lead
- **list_email_accounts**: List email accounts
- **pause_campaign**: Pause campaign
- **resume_campaign**: Resume campaign
- **list_campaigns**: List campaigns


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SmartLead** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the status of my 'Enterprise Q2' campaign?"

**🤖 AI Agent:**
> Campaign 'Enterprise Q2': 2,400 leads enrolled. Open rate: 54%, Reply rate: 7%, Bounce rate: 2.1%. Using 15 sending accounts with smart rotation. 168 positive replies received.

---

**👤 You:**
> "Check warm-up progress on my sending accounts."

**🤖 AI Agent:**
> 15 sending accounts total. 12 fully warmed (score 90+, ready for campaigns). 3 in progress (scores 55, 62, 78 — estimated 1-2 weeks to full warm-up).

---

**👤 You:**
> "Upload 500 new leads to the 'SaaS Founders' campaign."

**🤖 AI Agent:**
> 500 leads uploaded to 'SaaS Founders'. 487 accepted, 8 duplicates skipped, 5 invalid emails rejected. Campaign will automatically distribute new leads across your 12 active sending accounts.


## ❓ FAQ

**Q: How do I get my SmartLead API key?**
Log in to your SmartLead account at **app.smartlead.ai**. Click **Settings** in the left sidebar. Navigate to the **API** section. Your API key is displayed on this page — click **Copy**. Paste it into the configuration field below.

**Q: Can I manage hundreds of sending accounts?**
Yes. SmartLead is built for scale. Your AI agent can manage mailbox rotation, warm-up status, and daily sending limits across all accounts from a single conversation.

**Q: How does mailbox rotation work?**
SmartLead automatically distributes outgoing emails across your connected mailboxes, keeping each under safe daily sending limits. Your AI agent monitors this rotation and alerts you if any account approaches its limit.

**Q: Is SmartLead good for agencies?**
Yes. SmartLead is built specifically for cold email agencies with white-label capabilities, client management, and unlimited mailbox connections — all accessible through your AI agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smartlead](https://vinkius.com/mcp/smartlead)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SmartLead** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `smartlead` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SmartLead** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "smartlead": {
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
