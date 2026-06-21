# Gameball MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gameball)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Turn customers into loyal fans with gamified rewards, referral programs, and engagement challenges that drive repeat purchases.

## Description
Connect your **Gameball** loyalty and gamification account to any AI agent and simplify how you reward customer actions, manage player levels, and track points through natural conversation.

### What you can do

- **Player Oversight** — List all players and retrieve detailed metadata, including current loyalty level and total points.
- **Point Management** — Query real-time point balances and currency for any specific player ID.
- **Gamification Control** — List active challenges, badges, and rewards available in your loyalty ecosystem.
- **Event Automation** — Programmatically track player actions and events to trigger rewards or level progress via AI.
- **Loyalty Tiers** — Query defined loyalty levels and tiers to understand your customer distribution.
- **Discount Oversight** — List available coupons and promo codes currently active in your account.
- **Real-time Insights** — Verify player eligibility and track engagement metrics directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Gameball API Key (found in your account dashboard)
3. Start managing your gamified ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **E-commerce Managers** — quickly check customer point balances and award points for custom events via simple AI commands.
- **Marketing Teams** — monitor challenge progress and verify reward availability directly from the workspace.
- **Customer Success** — assist players with level inquiries and track engagement data via the AI assistant.


## Available Tools (8)
- **get_player_balance**: Check player points balance
- **get_player_details**: Get details for a specific player
- **list_challenges**: List active challenges
- **list_discount_coupons**: List available coupons
- **list_loyalty_levels**: List configured levels
- **list_players**: List Gameball players
- **list_rewards**: List available rewards
- **track_player_event**: Track a player action


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gameball** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the point balance for player 'user_10293'?"

**🤖 AI Agent:**
> I've retrieved the balance. Player user_10293 currently has 1,250 points (Value: $12.50). They are in the 'Silver Tier' and are 250 points away from reaching the Gold level. Shall I check their active challenges?

---

**👤 You:**
> "Award points for a 'Feedback Given' event to player 'user_88231'."

**🤖 AI Agent:**
> Event tracked! I've recorded the 'Feedback Given' action for user_88231 in Gameball. This has triggered a reward of 50 points and updated their progress for the 'Community Contributor' challenge.

---

**👤 You:**
> "List all active challenges in our loyalty program."

**🤖 AI Agent:**
> Fetching challenges... You have 5 active challenges: 'First Purchase', 'Refer a Friend', 'Weekly Login Streak', 'Write a Review', and 'Mobile App Install'. Would you like the point details for any of these?


## ❓ FAQ

**Q: Can I check a player's points balance via AI?**
Yes! Use the `get_player_balance` tool and provide the Player Unique ID. Your agent will retrieve the current points and currency for that specific user.

**Q: How do I award points for a specific action using the agent?**
Use the `track_player_event` action. Provide the Player ID and the Event Name (e.g., 'purchase_completed'). Gameball will process the event and trigger rewards based on your rules.

**Q: Is it possible to list all available rewards via AI?**
Absolutely. Use the `list_rewards` query. The agent will retrieve the full catalog of rewards, redemption options, and active point rules from your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gameball](https://vinkius.com/mcp/gameball)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gameball** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gameball` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gameball** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gameball": {
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
