# ReferralHero MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/referralhero)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate viral referral campaigns via ReferralHero — manage subscribers, rewards, and leaderboards with AI.

## Description
Connect your **ReferralHero** account to any AI agent and take full control of your viral growth orchestration and referral program management through natural conversation. ReferralHero provides a premier platform for building referral loops, and this integration allows you to retrieve subscriber metadata, monitor campaign leaderboards, and manage rewards directly from your chat interface.

### What you can do

- **Campaign & List Orchestration** — List all managed referral campaigns and retrieve detailed metadata, including creating and updating subscriber records programmatically.
- **Subscriber Lifecycle Management** — Access and monitor individual subscriber profiles and retrieve detailed performance metadata including point balances directly from the AI interface.
- **Leaderboard & Reward Intelligence** — Access real-time campaign leaderboards and monitor reward eligibility via natural language to drive program engagement.
- **Conversion & Referral Tracking** — Track conversion events and attribute referrals to specific subscribers to ensure your growth loops are always synchronized.
- **Operational Monitoring** — Track system activity and manage transaction metadata using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your ReferralHero API Token from your account settings
3. Start managing your referral campaigns from Claude, Cursor, or any MCP-compatible client

No more manual leaderboard exports or subscriber hunting. Your AI acts as a dedicated growth operations manager or referral coordinator.

### Who is this for?

- **Growth Marketers & Founders** — quickly retrieve campaign summaries and monitor subscriber growth without switching apps.
- **Marketing Operations Teams** — automate the management of referral points and track reward distributions via natural conversation.
- **Customer Success Teams** — streamline the retrieval of subscriber metadata and monitor referral history directly within the chat.


## Available Tools
- **add_points**: Add points to a subscriber
- **add_subscriber**: Add a new subscriber to a campaign
- **delete_subscriber**: Remove a subscriber from a campaign
- **get_leaderboard**: Get campaign leaderboard
- **get_list**: Get details for a specific campaign
- **get_rewards**: Get campaign rewards
- **get_subscriber**: Get details for a specific subscriber
- **list_lists**: List all referral campaigns (lists)
- **list_subscribers**: List subscribers for a campaign
- **list_transactions**: List recent transactions
- **track_conversion**: Track a referral conversion event
- **update_subscriber**: Update an existing subscriber


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ReferralHero** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active referral lists in my account."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 3 active lists including 'Early Access Launch' (UUID: list_123) and 'Refer-a-Friend'. Which one would you like to see the leaderboard for?

---

**👤 You:**
> "Show me the leaderboard of top referrers in my active campaign with their reward balances."

**🤖 AI Agent:**
> Top 10 referrers in "Growth Champions" campaign. #1: James Park with 47 verified referrals ($470 earned, $235 pending). #2: Lisa Wang with 34 referrals ($340 earned). #3: Alex Rivera with 28 referrals ($280 earned). #4-10: combined 89 referrals. Total campaign participants: 456. Active referrers (1+ referral): 234 (51%). Total rewards distributed: $4,560. Pending payouts: $1,230. Campaign viral coefficient: 1.4x. Average referrals per participant: 2.3.

---

**👤 You:**
> "Send a reminder email to all campaign participants who have not shared their referral link yet."

**🤖 AI Agent:**
> Reminder email sent to 222 inactive participants (those who joined but have 0 referrals). Subject: "Your referral link is waiting! Share & earn $10 per friend". Email includes their unique referral link, one-click social share buttons, and a progress bar showing how close they are to their first reward. Delivery: 218 delivered (98.2%). 4 bounced (invalid emails). Based on previous reminders, expect 15-20% to make their first share within 48 hours.


## ❓ FAQ

**Q: Can my AI automatically find the details and points for a specific subscriber by providing their ID?**
Yes! Use the `get_subscriber` tool with the List UUID and Subscriber ID. Your agent will respond with complete metadata, including referral counts and current point balances in seconds.

**Q: How do I find my ReferralHero API Token?**
Log in to your ReferralHero dashboard, navigate to **Account** > **API**, and you will find your unique secret token there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/referralhero](https://vinkius.com/mcp/referralhero)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ReferralHero** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `referralhero` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ReferralHero** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "referralhero": {
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
