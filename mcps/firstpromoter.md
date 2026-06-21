# FirstPromoter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/firstpromoter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage affiliates, track referrals, and handle rewards via AI agents with FirstPromoter.

## Description
Connect your **FirstPromoter** account to any AI agent and automate your affiliate and referral marketing operations through the Model Context Protocol (MCP). FirstPromoter is the all-in-one platform for SaaS companies to launch and manage affiliate, referral, and influencer programs. Now, you can manage your promoters and track conversions directly through natural conversation.

### What you can do

- **Promoter Management** — List all affiliates, fetch detailed performance metrics, and create new promoter profiles instantly.
- **Referral Tracking** — Monitor incoming leads and conversions to see which promoters are driving the most value.
- **Reward Processing** — List all rewards and commissions, and manually create new rewards for specific promoters.
- **Campaign Insights** — Access all your affiliate campaigns and fetch aggregate performance reports to optimize your strategy.
- **Performance Reporting** — Retrieve detailed reports for promoters and campaigns, including revenue and conversion data.
- **Payout Statistics** — Get a high-level overview of your payout statuses, including total paid and pending amounts.
- **Real-time Monitoring** — Fetch specific lead or conversion details to keep your marketing and finance teams aligned.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your FirstPromoter API Key and Account ID (found in your Settings > Integrations)
3. Start managing your affiliate programs from Claude, Cursor, or any MCP client

### Who is this for?

- **Affiliate Managers** — quickly check promoter stats or create manual rewards while reviewing program performance.
- **SaaS Founders** — get a quick overview of referral revenue and top-performing campaigns through simple AI commands.
- **Marketing Operations** — automate the gathering of conversion and lead data for internal marketing reports.


## Available Tools
- **create_promoter**: Create a new promoter
- **create_reward**: Create a new reward
- **get_campaign_report**: Get campaign performance report
- **get_lead**: Get lead details
- **get_payout_stats**: Get payout statistics
- **get_promoter_report**: Get promoter performance report
- **get_promoter**: Get promoter details
- **list_campaigns**: List affiliate campaigns
- **list_conversions**: List all conversions
- **list_leads**: List all leads
- **list_promoters**: List all promoters
- **list_rewards**: List rewards


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FirstPromoter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my top 10 promoters by revenue."

**🤖 AI Agent:**
> Retrieving top promoters... I found your top 10 affiliates, led by 'John Doe' ($5,400 revenue) and 'Jane Smith' ($4,200 revenue). Would you like the full details for any of them?

---

**👤 You:**
> "Show me the payout stats for this month."

**🤖 AI Agent:**
> Fetching payout statistics... Total paid this month: $12,500. Total pending payouts: $3,200. There are currently 15 promoters awaiting payment approval.

---

**👤 You:**
> "Create a new reward of $50.00 for promoter ID 'prom_456'."

**🤖 AI Agent:**
> Reward created! I've manually added a commission of $50.00 (5000 cents) to promoter ID 'prom_456'. The reward is now pending in their account.


## ❓ FAQ

**Q: How can I search for a specific promoter using the agent?**
You can use the 'list_promoters' tool and provide a search term in the 'q' parameter. This can be the promoter's name, email, or referral ID. The agent will return matching profiles.

**Q: Can I manually award a commission to an affiliate?**
Yes! The 'create_reward' tool allows you to manually create a reward for a specific promoter by providing their ID and the amount in cents.

**Q: Is it possible to see which campaigns are performing best?**
Absolutely. Use the 'get_campaign_report' tool to retrieve aggregate performance metrics across all your active campaigns, including referral counts and revenue generated.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/firstpromoter](https://vinkius.com/mcp/firstpromoter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FirstPromoter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `firstpromoter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FirstPromoter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "firstpromoter": {
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
