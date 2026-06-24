# Lemlist MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lemlist)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent with direct access to Lemlist — manage cold email campaigns, track lead engagement, and automate outreach without opening the Lemlist dashboard.

## Description
Connect **Lemlist** to your AI agent and manage your cold email outreach and lead engagement pipeline conversationally.

### What you can do

- **Campaign Management** — List, create, and monitor email campaigns with open rates, click rates, and reply metrics.
- **Lead Tracking** — Add leads to campaigns, check engagement statuses, and manage lead lists programmatically.
- **Sequence Analytics** — Pull step-by-step performance data for multi-touch email sequences.
- **Activity Feed** — Monitor recent opens, clicks, replies, and bounces across all campaigns.

### How it works

1. Subscribe to the Lemlist integration on the marketplace.
2. Generate an API key from your Lemlist account (Profile → Settings → Integrations → API section → Generate).
3. Ask your AI agent to manage campaigns, track leads, or pull engagement analytics.

### Who is this for?

- **SDR Teams** — Monitor outreach performance and lead engagement without switching between tools.
- **Growth Marketers** — Optimize email sequences based on real-time open, click, and reply data.
- **Agency Owners** — Track multi-client campaign performance from a single conversational interface.


## Available Tools (8)
- **get_team**: Get team info
- **list_campaigns**: List all campaigns
- **get_campaign**: Get campaign details
- **list_leads**: List campaign leads
- **add_lead**: Add lead to campaign
- **delete_lead**: Delete lead from campaign
- **pause_lead**: Pause a lead
- **resume_lead**: Resume a lead


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lemlist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the performance of my 'Q2 Outreach' campaign?"

**🤖 AI Agent:**
> Campaign 'Q2 Outreach': 450 leads contacted, 67% open rate, 12% click rate, 8% reply rate, 2% bounce rate. Top performing step: Email #2 (82% open rate). 36 positive replies received.

---

**👤 You:**
> "Add lead sarah@startup.io to the 'Series A Founders' campaign."

**🤖 AI Agent:**
> Lead added: sarah@startup.io → 'Series A Founders' campaign. She will receive the first email in the sequence based on your campaign schedule. Current position: Step 1 of 5.

---

**👤 You:**
> "Who replied to my emails this week?"

**🤖 AI Agent:**
> You received 14 replies this week across 3 campaigns. Positive replies: 9 (64%). Top responders: Mark at Acme Corp (interested in demo), Lisa at DataFlow (requesting pricing), and 7 others.


## ❓ FAQ

**Q: How do I get my Lemlist API key?**
Log in to your Lemlist account at **app.lemlist.com**. Click your **profile icon** (bottom left corner). Select **Settings**, then navigate to the **Integrations** tab. Look for the **API** section and click **Generate** to create a new API key. Copy the key immediately and save it securely — it is only shown once. Paste it into the configuration field below.

**Q: Can I check which leads opened my emails today?**
Yes. Ask your AI agent 'Who opened my emails today?' and it returns a list of leads with their email addresses, campaign names, open timestamps, and total open counts — giving your SDR team warm lead signals in real-time.

**Q: Can my agent add new leads to an existing campaign?**
Yes. Provide the lead's email, first name, and any custom variables, and your AI agent adds them directly to any active campaign — they'll automatically enter the sequence at step 1. Perfect for sales teams who find prospects and want to start outreach immediately.

**Q: What engagement metrics can I track?**
Your AI agent can pull opens, clicks, replies, bounces, and unsubscribes per campaign — plus step-by-step analytics showing which emails in your sequence perform best. Perfect for optimizing subject lines, send times, and follow-up cadences.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lemlist](https://vinkius.com/mcp/lemlist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lemlist** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lemlist` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lemlist** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lemlist": {
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
