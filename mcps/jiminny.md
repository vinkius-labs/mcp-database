# Jiminny MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jiminny)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Coach your sales team with conversation intelligence that records calls, identifies winning behaviors, and forecasts deals.

## Description
Connect your **Jiminny** account to any AI agent and take full control of your sales conversation intelligence and automated coaching workflows through natural conversation.

### What you can do

- **Call Portfolio Orchestration** â€” List and manage your entire database of call recordings and transcripts programmatically, retrieving detailed speaker metadata
- **Meeting Intelligence Architecture** â€” Programmatically query and monitor meeting insights and key moments to maintain a perfectly coordinated sales audit trail
- **Rep Performance Monitoring** â€” Access real-time activity metrics for your sales team and track improvement trends directly through your agent for instant reporting
- **Metadata Management** â€” Programmatically retrieve talk-to-listen ratios and filler word counts to maintain a perfectly coordinated coaching record
- **Operational Monitoring** â€” Verify account-level API connectivity and monitor call ingestion volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Jiminny dashboard (Settings > API)
3. Start orchestrating your sales growth from Claude, Cursor, or any MCP client

No more manual reviewing of long call recordings or missing coaching opportunities. Your AI acts as your dedicated sales coach and conversation architect.

### Who is this for?

- **Sales Managers** â€” instantly retrieve call summaries and monitor rep improvement using natural language commands
- **Enablement Leads** â€” verify individual meeting metadata and track coaching activity without leaving your creative workspace
- **Developers** â€” integrate high-speed Jiminny conversation data into custom CRM and BI tools through simple AI queries


## Available Tools (10)
- **check_jiminny_status**: Verify Jiminny API connectivity
- **get_action_items**: Get action items from a call
- **get_activity**: Get activity details
- **get_call_stats**: Get aggregate call analytics
- **get_coaching_stats**: Get coaching stats for a user
- **get_transcript**: Get call transcript
- **get_user**: Get user details
- **list_activities**: List all calls and meetings
- **list_teams**: List all teams
- **list_users**: List all team members


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jiminny** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all calls recorded today in Jiminny."

**🤖 AI Agent:**
> 12 calls recorded today. The longest was a 45-minute demo by Sarah Chen with Acme Corp. Would you like to see the transcript or action items from any call?

---

**👤 You:**
> "Get the transcript and action items from call ACT-9421."

**🤖 AI Agent:**
> Call ACT-9421 transcript retrieved (42 min, 3 speakers). I found 4 action items: send proposal by Friday, schedule follow-up, share pricing doc, and intro to engineering team. Want me to format these as tasks?

---

**👤 You:**
> "Show coaching stats for user USR-201."

**🤖 AI Agent:**
> User USR-201 (Sarah Chen): Average call score 8.2/10, talk ratio 42%, 15 calls this week. Improvement trend: +12% over last month. Top strength: discovery questions. Would you like team-wide analytics?


## ❓ FAQ

**Q: How do I access call transcripts via AI?**
Use the `get_transcript` tool with the activity ID to retrieve the full transcript with speaker identification and timestamps.

**Q: Can my agent extract action items from calls?**
Yes. Use `get_action_items` to retrieve all AI-detected follow-ups and tasks from any recorded conversation.

**Q: How do I review coaching metrics for my team?**
Use `get_coaching_stats` with the user ID to see call scores, framework ratings, and improvement trends for any team member.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jiminny](https://vinkius.com/mcp/jiminny)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jiminny** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jiminny` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jiminny** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jiminny": {
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
