# Bonusly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bonusly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Recognize and reward your team via Bonusly — give bonuses, track points, and view leaderboards directly from any AI agent.

## Description
Connect your **Bonusly** employee recognition account to any AI agent and orchestrate your team culture and reward workflows through natural conversation.

### What you can do

- **Peer Recognition** — Instantly give bonuses to colleagues with custom reasons and hashtags representing company values.
- **Bonus Oversight** — List recent bonuses and retrieve detailed information for specific recognition events.
- **User & Profile Management** — Access employee profiles and check your own point balance and history.
- **Reward Tracking** — Monitor recent redemptions to see how your team is spending their earned points.
- **Culture Insights** — List company values, popular hashtags, and view the real-time recognition leaderboard.

### How it works

1. Subscribe to this server
2. Enter your Bonusly API Access Token
3. Start rewarding your team from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Team Leads** — quickly recognize members for great work without leaving their workflow tools.
- **HR Managers** — monitor employee engagement and company value alignment using natural language.
- **Employees** — check their point balances and give quick shout-outs to peers.


## Available Tools
- **get_bonus**: Get details of a specific bonus
- **get_leaderboard**: Get the recognition leaderboard
- **get_my_profile**: Get the profile of the authenticated user
- **get_user**: Get profile details for an employee
- **give_bonus**: Give a recognition bonus to an employee
- **list_bonuses**: List recent employee bonuses
- **list_hashtags**: List popular hashtags
- **list_redemptions**: List recent reward redemptions
- **list_users**: List all employees
- **list_company_values**: List company values and hashtags


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bonusly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give +10 to sarah@example.com for helping with the client presentation #teamwork."

**🤖 AI Agent:**
> Recognition posted! I've given 10 points to Sarah with the reason: 'helping with the client presentation #teamwork'.

---

**👤 You:**
> "What is my current Bonusly balance?"

**🤖 AI Agent:**
> You currently have 150 points available to give and 450 points that you've received and can redeem for rewards.

---

**👤 You:**
> "Show the recent bonuses in the company."

**🤖 AI Agent:**
> Retrieving recent bonuses... Notable recognition includes Mark giving to Alice for 'great code review' and Janet giving to the team for 'launching the new site'.


## ❓ FAQ

**Q: Can I give a bonus to a colleague using the agent?**
Yes! Use the `give_bonus` tool with the recipient's email, the amount of points, and a reason including hashtags like #teamwork. Your agent will post the recognition to Bonusly instantly.

**Q: How do I check my current point balance?**
Simply ask the agent to `get_my_profile`. It will retrieve your personal Bonusly profile, showing your available giving and receiving point balances.

**Q: Can I see who the top recognized employees are?**
Yes. Use the `get_leaderboard` tool to retrieve the current recognition rankings, showing the top givers and receivers in your organization.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bonusly](https://vinkius.com/mcp/bonusly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bonusly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bonusly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bonusly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bonusly": {
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
