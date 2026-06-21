# Genius Referrals MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/genius-referrals)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage referral programs, track advocates, and oversee rewards via AI agents with Genius Referrals.

## Description
Connect your **Genius Referrals** account to any AI agent to automate your referral marketing and advocate engagement through the Model Context Protocol (MCP). Genius Referrals is a robust platform that helps brands build sophisticated word-of-mouth campaigns. This MCP server enables you to manage your advocate database, track referral conversions, and retrieve reward distributions directly through natural conversation.

### Key Features

- **Advocate Management** — List all advocates in your program, retrieve detailed profile metadata, and programmatically register new promoters.
- **Referral Tracking** — Monitor all tracked referral conversions (signups, purchases) and check their current status instantly.
- **Campaign Discovery** — Access your configured referral campaigns and fetch detailed rules and reward structures.
- **Reward Oversight** — List awarded bonuses and rewards distributed to advocates to understand your program's performance.
- **Redemption Requests** — Monitor requests from advocates to claim or payout their earned rewards.
- **Performance Insights** — Identify your top-performing advocates and track the total referral count for your business.
- **Real-time Synchronization** — Keep your referral marketing data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Genius Referrals API Token (found in Settings > API Access)
3. Start managing your referral campaigns from Claude, Cursor, or any MCP client

### Who is this for?

- **Growth Marketers** — quickly check the status of a specific referral conversion or list top advocates without manual dashboard navigation.
- **Customer Success Ops** — automate the registration of new advocates and verify reward distributions via simple AI commands.
- **Operations Managers** — monitor redemption requests and audit program bonuses seamlessly.


## Available Tools (12)
- **verify_api_connection**: Check connection
- **register_advocate**: Register new advocate
- **log_referral_conversion**: g. signup or purchase).

Track a referral
- **get_my_account**: Get account identity
- **get_advocate_details**: Get advocate metadata
- **get_campaign_details**: Get campaign metadata
- **list_program_advocates**: List advocates
- **list_awarded_bonuses**: List earned rewards
- **list_referral_campaigns**: List campaigns
- **list_payout_requests**: List redemption requests
- **list_tracked_referrals**: List referral events
- **list_top_performers**: List top advocates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Genius Referrals** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active referral campaigns in my account."

**🤖 AI Agent:**
> Retrieving campaigns... I found 2 active campaigns: 'Fall Friends & Family' and 'Annual Loyalty Program'. Would you like the reward rules for either?

---

**👤 You:**
> "Register 'Jane Smith' (jane@example.com) as a new advocate."

**🤖 AI Agent:**
> Advocate registered! Jane Smith has been successfully added to your referral program. Her personal referral code is 'JANE-SMITH-123'.

---

**👤 You:**
> "Show me the 5 most recent referral conversions."

**🤖 AI Agent:**
> Fetching referrals... I found 5 recent conversions. 3 are currently 'Verified' and 2 are 'Pending' verification. Would you like to see the associated bonus amounts?


## ❓ FAQ

**Q: How do I get an API Token for Genius Referrals?**
Log in to your Genius Referrals dashboard, click your name in the top-left corner, and select 'API Access' to find your API token.

**Q: Can I manually track a referral conversion via the agent?**
Yes! Use the 'log_referral_conversion' tool. You must provide the advocate's email and the email of the person they referred to trigger the tracking logic.

**Q: How do I register a new advocate through the chat?**
Use the 'register_advocate' tool and provide the person's email and full name. The agent will add them to your program and generate their referral link.

**Q: Is it possible to see who my best advocates are?**
Yes, the 'list_top_performers' tool retrieves a list of advocates sorted by their referral count, helping you identify your most active promoters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/genius-referrals](https://vinkius.com/mcp/genius-referrals)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Genius Referrals** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `genius-referrals` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Genius Referrals** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "genius-referrals": {
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
