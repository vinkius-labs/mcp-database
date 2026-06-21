# FynCom MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fyncom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Reward customer attention with micro-payments and nano-rewards that boost survey completion and email engagement rates.

## Description
Connect your **FynCom** account to any AI agent and take full control of your user incentives and reward operations through natural conversation.

### What you can do

- **Reward Orchestration** — Send instant cryptocurrency or fiat rewards to users or email addresses programmatically to incentivize engagement and feedback
- **Campaign Management** — Access and monitor your active reward campaigns and retrieve detailed performance and lead metadata in real-time
- **Lead Engagement Tracking** — Add leads to specific reward workflows programmatically from your AI agent to trigger automated incentives and follow-ups
- **Wallet Intelligence** — Check your real-time rewards wallet balance directly through your agent to ensure uninterrupted delivery of user incentives
- **Transaction Oversight** — Get a comprehensive overview of your reward history and campaign health using natural language commands

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your FynCom dashboard (Settings > API)
3. Start managing your user rewards from Claude, Cursor, or any MCP client

No more manual payment processing for small incentives. Your AI acts as your dedicated rewards and engagement coordinator.

### Who is this for?

- **Growth Marketers** — automate the delivery of incentives for survey completions and product feedback using natural language queries
- **Customer Success Managers** — reward key customer actions and track engagement patterns more efficiently without leaving your workspace
- **Product Developers** — integrate real-time reward systems and incentive intelligence into custom applications through automated AI actions


## Available Tools (6)
- **add_reward_lead**: Pass data in JSON.

Add a lead to a reward campaign
- **get_wallet_balance**: Check current rewards wallet balance
- **get_campaign_details**: Get specific campaign details
- **list_reward_campaigns**: List active reward campaigns
- **list_reward_history**: List history of sent rewards
- **send_reward**: Pass data as a JSON string.

Send a reward or incentive


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FynCom** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active reward campaigns in FynCom."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 3 active initiatives, including 'Beta Tester Rewards' (ID: camp_123) and 'Feedback Incentives' (ID: camp_456). Which one would you like to add a lead to?

---

**👤 You:**
> "Send a $5 reward to 'user@example.com'."

**🤖 AI Agent:**
> Reward sent successfully! I've delivered the $5.00 incentive to 'user@example.com' (Transaction ID: fyn_992). The user will receive their reward notification shortly.

---

**👤 You:**
> "Check my FynCom wallet balance."

**🤖 AI Agent:**
> Your current rewards wallet balance is $250.00. You have sufficient funds to cover approximately 50 more rewards of $5.00 each.


## ❓ FAQ

**Q: How do I find my FynCom API Key?**
Log in to your FynCom dashboard and navigate to the **Settings** > **API** section to generate or copy your unique key.

**Q: Can I check my wallet balance via AI?**
Yes! Use the `get_wallet_balance` tool to retrieve your current rewards budget and ensured you have sufficient funds for your campaigns.

**Q: How do I add a lead to a reward campaign?**
Use the `add_reward_lead` tool by providing the `campaign_id` and a JSON string with the lead's email and other required details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fyncom](https://vinkius.com/mcp/fyncom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FynCom** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fyncom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FynCom** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fyncom": {
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
