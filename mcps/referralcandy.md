# ReferralCandy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/referralcandy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Connect your AI agents to ReferralCandy to manage referral programs, track advocates, register purchases, and analyze campaign performance.

## Description
Give your AI agent full programmatic control over your ReferralCandy ecosystem. With 16 tools tailored for referral marketing, your agent can instantly track referrals by period, register attributed purchases, identify top advocates, monitor pending rewards, manage campaigns, and send referral invitations directly from your natural language workspace.

### What you can do
- List and filter referrals by period
- Register purchases to trigger rewards
- Identify and manage top-performing advocates
- Monitor pending referral payouts
- Configure campaigns and send invites
- Access overall program statistics

### How it works
1. Subscribe to this server
2. Enter your ReferralCandy API Keys (found in your developer settings)
3. Let your AI agents start managing your referral operations via Vinkius

### Who is it for?
Designed for marketing teams, e-commerce operators, and growth hackers who need instant, conversational access to affiliate and referral performance metrics.


## Available Tools
- **check_referralcandy_status**: Verify connectivity
- **get_campaign**: Get campaign details
- **get_referral**: Get referral details
- **get_referrer**: Get advocate profile
- **get_stats**: Get program stats
- **get_top_referrers**: Get top advocates
- **list_campaigns**: List campaigns
- **list_invites**: List sent invites
- **list_pending_rewards**: List pending rewards
- **list_purchases**: List referred purchases
- **list_referrals_by_period**: List referrals by period
- **list_referrals**: List all referrals
- **list_referrers**: List all advocates
- **list_rewards**: List all rewards
- **register_purchase**: Register a purchase
- **send_invite**: Send a referral invite


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ReferralCandy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you find the top referrers in my ReferralCandy program for the last month?"

**🤖 AI Agent:**
> I've fetched your top advocates. The highest performer is 'Sarah Jenkins' with 42 successful referrals, generating $1,200 in revenue. Would you like me to send her a special campaign invite?

---

**👤 You:**
> "Register a purchase of $150.00 for order #90210 by customer@example.com."

**🤖 AI Agent:**
> Executing the purchase registration... The purchase for order #90210 has been successfully logged. ReferralCandy has attributed this to the advocate 'Michael T.' and a pending reward of $15 has been queued.

---

**👤 You:**
> "List all pending referral rewards that need to be processed this week."

**🤖 AI Agent:**
> Running the query... I found 8 pending rewards awaiting processing. Notable payouts include $50 for 'Alex' and $25 for 'Maria'. Would you like the full breakdown of these pending payouts?


## ❓ FAQ

**Q: Can my AI automatically register a new purchase to trigger a referral reward?**
Yes! Use the `register_purchase` tool providing the buyer's email, order amount, and order ID. Your agent will send this data to ReferralCandy, triggering the referral attribution and payout flow instantly.

**Q: How do I easily find out who my best performing advocates are?**
Simply ask the agent to run the `get_top_referrers` action. It will compile your highest-performing ambassadors ranked by total successful referrals and the total revenue they generated for your store.

**Q: Can I check if a specific customer has any pending referral rewards?**
Absolutely. By using the `list_pending_rewards` tool and filtering by the customer's email, your agent can instantly fetch their reward status and payout timeline without you needing to open the dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/referralcandy](https://vinkius.com/mcp/referralcandy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ReferralCandy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `referralcandy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ReferralCandy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "referralcandy": {
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
