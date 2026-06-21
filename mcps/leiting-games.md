# Leiting Games MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/leiting-games)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Leading game publisher and developer platform — manage submissions, track performance, and audit compliance via AI.

## Description
Empower your AI agent to manage your publishing journey with **Leiting Games**, the premier platform for indie and roguelike game development in China. By connecting Leiting Games to your agent, you transform complex game submissions, partner analytics, and compliance auditing into a natural conversation. Your agent can instantly list your published games, retrieve real-time operational status, analyze marketing data, and even audit your compliance with anti-addiction regulations without you needing to navigate technical partner portals. Whether you are an indie creator or an established studio, your agent acts as a real-time publishing assistant, ensuring your games reach their full potential in the Chinese market.

### What you can do

- **Game Management** — List all your published games and monitor their real-time operational and publishing status.
- **Proposal Submission** — Submit new game titles and genre information for review directly through the chat interface.
- **Marketing Analytics** — Retrieve performance data and user acquisition metrics to track your marketing efficiency.
- **Compliance Auditing** — Audit the compliance score of your games, including real-name authentication and anti-addiction status.
- **SDK Access** — Browse the latest SDK releases and versions to keep your game integration up to date.
- **Partner Insights** — Monitor overall partner statistics and administrative audit logs for your account.

### How it works

1. Subscribe to this server
2. Enter your Leiting Games Partner Token
3. Start managing your publishing workflow through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Independent Game Developers** — manage your publishing process and track performance from your AI-powered workspace.
- **Publishing Managers** — audit compliance and monitor game statuses across a large portfolio through natural language.
- **Business Developers** — track collaborations and marketing analytics for upcoming and active game titles.
- **Technical Integrators** — monitor SDK releases and version history to streamline your development pipeline.


## Available Tools (10)
- **get_audit_logs**: Get account audit logs
- **get_compliance_status**: Check compliance status
- **get_developer_profile**: Get developer profile info
- **get_game_status**: Get game publishing status
- **get_marketing_data**: Get marketing analytics
- **get_partner_stats**: Get partner statistics summary
- **list_collaborations**: List active collaborations
- **list_games**: List published games
- **list_sdk_releases**: List SDK releases
- **submit_game**: Submit a new game for review


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Leiting Games** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my games published with Leiting."

**🤖 AI Agent:**
> I've retrieved your game list from Leiting. You have 3 active titles: 'Roguelike Dungeon', 'Taoist Cultivation', and 'Slime Adventure'. All are currently in 'Normal' operational status.

---

**👤 You:**
> "Check the compliance status for 'Roguelike Dungeon'."

**🤖 AI Agent:**
> Compliance audit for 'Roguelike Dungeon' is complete. Compliance score: 98/100. Real-name authentication and anti-addiction modules are active. No major issues found.

---

**👤 You:**
> "Submit a new game title 'Mech Warrior' (RPG) for review."

**🤖 AI Agent:**
> Done! I've submitted 'Mech Warrior' (Genre: RPG) to the Leiting Games review team. You can track the submission status using ID: SUB-9920.


## ❓ FAQ

**Q: How do I obtain a Leiting Partner Token?**
You must register as a developer or publisher on the Leiting Games cooperation platform. Once your application is reviewed and approved, you can generate your Partner Token in the dashboard.

**Q: Can I submit a new game for review through the agent?**
Yes! Use the `submit_game` tool. You will need to provide the title and genre. This initiates the review process with the Leiting publishing team.

**Q: How does the compliance audit tool work?**
The `get_compliance_status` tool checks if your game is correctly integrated with China's mandatory real-name authentication and anti-addiction systems, providing a safety score.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/leiting-games](https://vinkius.com/mcp/leiting-games)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Leiting Games** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `leiting-games` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Leiting Games** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "leiting-games": {
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
