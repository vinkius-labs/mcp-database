# Gong MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gong)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Unlock revenue intelligence by analyzing calls, transcripts, and customer interactions.

## Description
Connect your **Gong** organizational account to your AI agent and gain deep insights into your sales conversations and customer interactions. Use natural language to query transcripts, analyze team performance, and track deal progress.

### What you can do

- **Call Analysis** — List recent calls, search for specific keywords, and retrieve full transcripts for deep-dive analysis
- **User & Team Insights** — Monitor team activity and retrieve interaction statistics to understand coaching opportunities
- **Account Management** — Access CRM accounts linked in Gong to see the full context of every deal and relationship
- **Tracker Monitoring** — List and monitor configured trackers to identify recurring themes and competitive mentions in real-time
- **Scorecards & Reviews** — Access call scorecards to see how conversations align with your organization's sales methodology

### How it works

1. Subscribe to this server
2. Enter your Gong Access Key and Access Key Secret (found in your Gong API settings)
3. Start querying your revenue intelligence data from Claude, Cursor, or any MCP-compatible client

Your AI acts as a dedicated sales analyst, helping you identify what separates your top closers from the rest of the team without manual auditing.

### Who is this for?

- **Sales Managers** — instantly summarize recent high-stakes calls and check team compliance with sales scripts
- **Revenue Operations** — audit account interactions and track the adoption of new messaging across the organization
- **Enablement Teams** — identify coaching moments by analyzing interaction stats and scorecard results at scale


## Available Tools
- **get_account**: Get details for a specific account
- **get_call_media**: Get the media/recording details for a call
- **get_call**: Get details for a specific call
- **get_interaction_stats**: Get aggregated interaction statistics
- **get_transcript**: Retrieve the transcript of a call
- **get_user**: Get details for a specific user
- **list_accounts**: List CRM accounts linked in Gong
- **list_calls**: List Gong calls
- **list_scorecards**: List scorecards used for call reviews
- **list_trackers**: List configured trackers (keywords/phrases)
- **list_users**: List Gong users
- **search_calls**: Search for calls with complex filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gong** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Summarize the transcript for call ID 839201."

**🤖 AI Agent:**
> Analyzing transcript... The call involved a discussion about pricing tiers and API integration. The customer expressed interest in the Enterprise plan but requested more details on the security audit process. Key takeaway: Follow up with the SOC2 report.

---

**👤 You:**
> "Which calls last week mentioned our competitor 'CompetitorX'?"

**🤖 AI Agent:**
> Searching trackers... I found 3 calls where 'CompetitorX' was mentioned. In call #93021, the customer compared their feature set to ours. Would you like me to pull the specific snippets from those transcripts?

---

**👤 You:**
> "Show me the interaction stats for user Marcus R. for the last 30 days."

**🤖 AI Agent:**
> Retrieving metrics... Marcus R. had 45 calls with an average duration of 22 minutes. His 'Talk-to-Listen' ratio was 45%, which is within the target range. However, his longest monologue increased by 10% compared to last month.


## ❓ FAQ

**Q: Can I search for specific keywords across all my company's recorded calls?**
Yes! Use the `search_calls` tool to filter calls by content, participants, or specific trackers. You can then use `get_transcript` to analyze exactly how those terms were used in context.

**Q: Does this integration provide access to the actual audio or video recording?**
The `get_call_media` tool provides details about the media associated with a call. For security reasons, the AI primarily analyzes the text-based transcript and metadata, but it can provide links to the recording on the Gong platform.

**Q: How current is the data retrieved by the AI agent?**
The integration queries Gong's API in real-time. As soon as a call is processed and available in your Gong dashboard, it can be retrieved and analyzed by your AI agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gong](https://vinkius.com/mcp/gong)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gong** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gong` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gong** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gong": {
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
