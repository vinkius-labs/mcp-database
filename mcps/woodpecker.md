# Woodpecker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/woodpecker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Equip your AI agent with direct access to Woodpecker — manage cold email sequences, track prospect engagement, and monitor deliverability without opening the Woodpecker platform.

## Description
Connect **Woodpecker** to your AI agent and manage your B2B cold email automation platform conversationally.

### What you can do

- **Campaign Management** — Create, run, pause, and stop email campaigns with multi-step follow-up sequences.
- **Prospect Tracking** — Add prospects, check reply statuses, and manage bounces and opt-outs.
- **Analytics** — Pull open rates, click rates, reply rates, and bounce metrics per campaign.
- **Deliverability Monitoring** — Track sending limits, warm-up progress, and inbox placement.

### How it works

1. Subscribe to the Woodpecker integration on the marketplace.
2. Generate an API key from your Woodpecker account (Settings → API keys → Create new key).
3. Ask your AI agent to manage campaigns, track prospects, or check deliverability.

### Who is this for?

- **B2B Sales Teams** — Automate and monitor cold email outreach with personalized follow-up sequences.
- **Agencies** — Manage email campaigns across multiple client accounts from one interface.
- **Founders** — Run lean outreach operations without a dedicated SDR team.


## Available Tools (8)
- **list_webhooks**: List webhooks
- **list_campaigns**: List campaigns
- **get_campaign**: Get campaign
- **list_prospects**: List prospects
- **add_prospect**: Add prospect
- **get_campaign_stats**: Get campaign stats
- **pause_campaign**: Pause campaign
- **resume_campaign**: Resume campaign


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Woodpecker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show campaign stats for 'VP Engineering Outreach'."

**🤖 AI Agent:**
> Campaign 'VP Engineering Outreach': 320 prospects, 58% open rate, 11% reply rate, 2% bounce rate. Step 2 (follow-up) has the highest reply rate at 15%. 35 positive replies total.

---

**👤 You:**
> "Add 20 new prospects to my active campaign."

**🤖 AI Agent:**
> 20 prospects added to 'VP Engineering Outreach'. 19 accepted, 1 skipped (email already in blacklist). First emails will be sent based on your daily sending schedule.

---

**👤 You:**
> "Who replied to my campaigns this week?"

**🤖 AI Agent:**
> 18 replies this week across 3 campaigns. 12 positive (67%), 4 not interested, 2 auto-replies. Notable: CTO at DataFlow requested a demo.


## ❓ FAQ

**Q: How do I get my Woodpecker API key?**
Log in to your Woodpecker account at **app.woodpecker.co**. Navigate to **Settings** (gear icon). Click on **API keys** in the left menu. Click **Create new key**, give it a descriptive name, and copy the generated key. Paste it below. API access is available on all Woodpecker plans.

**Q: Can I automate multi-step follow-up sequences?**
Yes. Woodpecker specializes in automated follow-up sequences. Your AI agent can create campaigns with up to 7 follow-up steps, each with customizable delays and personalization variables.

**Q: Does it protect my sender reputation?**
Yes. Woodpecker includes built-in bounce detection, auto-blacklisting, and sending throttling. Your AI agent can monitor these safety metrics and alert you if deliverability drops below healthy thresholds.

**Q: Can I use it for agency clients?**
Yes. Woodpecker offers an Agency plan with multi-client management. Each API key is scoped to your account, and you can manage campaigns for all clients from your AI agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/woodpecker](https://vinkius.com/mcp/woodpecker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Woodpecker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `woodpecker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Woodpecker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "woodpecker": {
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
