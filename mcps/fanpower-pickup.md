# FanPower (PickUp) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fanpower-pickup)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Drive fan engagement via FanPower (PickUp) — manage interactive questions, track fan picks, and monitor rewards directly through your AI agent.

## Description
Connect your **FanPower (now PickUp)** engagement account to any AI agent and take full control of your interactive sports and esports content through natural conversation.

### What you can do

- **Interactive Content Management** — List all engagement questions and fetch detailed configurations for your interactive widgets
- **Fan Pick Tracking** — List and inspect individual fan answers (picks) to understand audience predictions and sentiment
- **Audience Profiling** — Retrieve fan profiles and participation history to build your zero-party database
- **Gamification & Rewards** — Monitor available rewards, achievements, and leaderboard rankings natively
- **Event Coordination** — List and inspect sports/esports events associated with your interactive content
- **Identity Context** — Verify your API user profile and authorized access levels flawlessly

### How it works

1. Subscribe to this server
2. Enter your FanPower (PickUp) API Key
3. Start managing your fan engagement from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sports Media Publishers** — monitor question performance and fan participation without leaving your workflow
- **Engagement Managers** — track leaderboard trends and reward distribution through simple natural language queries
- **Esports Teams** — pull fan data and participation metrics directly into your AI-powered marketing stack


## Available Tools
- **get_event_details**: Get details for a specific event
- **get_fan_profile**: Get the profile of a specific fan
- **get_leaderboard**: Get the fan leaderboard for engagement scores
- **get_me**: Get current API user identity
- **get_pick_details**: Get details for a specific fan pick
- **get_question**: Get details for a specific engagement question
- **get_reward_details**: Get details for a specific reward
- **list_events**: List sports or esports events with interactive content
- **list_fans**: List registered fans and participants
- **list_picks**: List fan picks (answers) for interactive content
- **list_questions**: List all interactive fan engagement questions
- **list_rewards**: List available rewards and achievements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FanPower (PickUp)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active engagement questions on FanPower."

**🤖 AI Agent:**
> I've retrieved your active questions. You have 'Who will win the NBA Finals?' (ID: 101) and 'MVP of the Match?' (ID: 102) currently live. Would you like to see the engagement score for any of these?

---

**👤 You:**
> "Show me the top 5 fans on the leaderboard."

**🤖 AI Agent:**
> Fetching leaderboard... The top 5 fans are 'Fan_123' (Score: 1200), 'SuperFan_99' (Score: 1150), and 'GamerX' (Score: 1100). Shall I retrieve the profile details for any of them?

---

**👤 You:**
> "List the latest fan picks for the Lakers vs Celtics game."

**🤖 AI Agent:**
> Analyzing picks for the event... I found 50 new picks. 70% of fans predicted a Lakers victory, while 30% went with the Celtics. Would you like to see the individual responses?


## ❓ FAQ

**Q: How do I obtain my FanPower (PickUp) API Key?**
You can request an API Key from your account manager at PickUp or through their developer portal at wiki.playpickup.com.

**Q: Can I see the results of individual fan predictions?**
Yes! The `list_picks` and `get_pick_details` tools allow you to retrieve individual answers submitted by fans for any interactive content.

**Q: Is it possible to monitor the fan leaderboard?**
Absolutely. Use the `get_leaderboard` tool to see the top-performing fans based on their participation and prediction accuracy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fanpower-pickup](https://vinkius.com/mcp/fanpower-pickup)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FanPower (PickUp)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `fanpower-pickup` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FanPower (PickUp)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fanpower-pickup": {
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
