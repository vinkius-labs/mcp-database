# Friendbuy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/friendbuy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage referral programs, track purchases, and oversee rewards via AI agents with Friendbuy.

## Description
Connect your **Friendbuy** account to any AI agent to automate your referral programs and customer loyalty workflows through the Model Context Protocol (MCP). Friendbuy is a high-growth referral marketing platform that powers word-of-mouth campaigns for leading brands. This MCP server enables you to track referral events, log conversions, and retrieve reward distributions directly through natural conversation.

### Key Features

- **Referral Rewards Tracking** — List all distributed referral rewards and filter them by advocate to understand who your top promoters are.
- **Conversion Logging** — Post purchase and signup events programmatically to trigger the referral reward lifecycle.
- **Code Generation & Verification** — Create personal referral codes for customers and check their active statuses instantly.
- **Purchase History** — Retrieve a list of all tracked purchases that have been attributed to referral campaigns.
- **Webhook Monitoring** — List configured webhooks to ensure your internal systems are receiving real-time reward notifications.
- **API Health Checks** — Verify your connection to both the Merchant API and Developer API v2 environments seamlessly.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Friendbuy Access Key and Secret Key (found in your Developer Settings)
3. Start managing your referral campaigns from Claude, Cursor, or any MCP client

### Who is this for?

- **Growth Marketers** — quickly check the status of a specific referral code or list recent rewards without navigating the dashboard.
- **E-commerce Ops** — automate the logging of offline or subscription purchases to ensure advocates get rewarded.
- **Customer Support** — verify if a specific customer's referral resulted in a successful conversion via simple AI commands.


## Available Tools
- **get_referral_code_status**: Check code status
- **create_referral_code**: Generate share code
- **check_api_connection**: Verify API access
- **list_tracked_purchases**: List tracked purchases
- **list_referral_rewards**: List awarded referrals
- **list_webhooks**: List webhook configs
- **track_conversion_purchase**: Log a purchase
- **track_conversion_signup**: Log a signup


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Friendbuy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all recent referral rewards distributed."

**🤖 AI Agent:**
> Retrieving rewards... I found 5 recent referral rewards, including a $20 account credit for 'advocate@example.com'.

---

**👤 You:**
> "Generate a new referral code for customer 'user_123' (jane@email.com)."

**🤖 AI Agent:**
> Code generated! Jane's unique referral code is 'JANE-REF-99'. She can now share this with friends to earn rewards.

---

**👤 You:**
> "Track a $50 purchase for order 'ORD-987' from 'friend@email.com' using code 'JANE-REF-99'."

**🤖 AI Agent:**
> Purchase tracked successfully! The $50 conversion for order ORD-987 has been logged, and the referral reward logic for advocate Jane has been triggered.


## ❓ FAQ

**Q: How do I get my API Keys for Friendbuy?**
Log in to your Friendbuy account, go to Settings > Developer, and you will find your Access Key and Secret Key.

**Q: Can I manually log a purchase through the agent?**
Yes! Use the 'track_conversion_purchase' tool. Provide the Order ID, amount, and customer email. If you include the 'referralCode', it will trigger the advocate's reward.

**Q: How do I verify if a referral code is still valid?**
Use the 'get_referral_code_status' tool. The agent will check the Developer API and return the active status and associated reward value.

**Q: Is it possible to list webhooks?**
Yes, the 'list_webhooks' tool retrieves all active webhook configurations so you can verify where real-time reward notifications are being sent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/friendbuy](https://vinkius.com/mcp/friendbuy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Friendbuy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `friendbuy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Friendbuy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "friendbuy": {
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
