# Cursor Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cursor-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Track team AI coding metrics from Cursor — agent edit acceptance rates, tab autocomplete stats, daily active users, model usage, MCP/command/plan/skill adoption, and team leaderboards from any AI agent.

## Description
Connect your **Cursor Analytics** API key to any AI agent and gain full visibility into your team's AI-assisted coding activity through natural conversation.

### What you can do

- **Agent Edit Metrics** — Track AI-suggested code edits including suggested diffs, accepted diffs, rejected diffs, and lines suggested/accepted to measure AI coding acceptance rates
- **Tab Autocomplete Usage** — Monitor tab autocomplete suggestions, accepts, rejects, and lines accepted to understand how your team leverages inline completions
- **Daily Active Users** — Get DAU counts with breakdowns by CLI usage, cloud agent activity, and Bugbot usage to track adoption trends
- **Client Version Distribution** — See which Cursor client versions your team is running to plan upgrade rollouts and identify outdated installations
- **Model Usage Breakdown** — Understand which AI models your team prefers with messages sent and active users per model per day
- **Top File Extensions** — Discover the top 5 file extensions per day ranked by suggestion volume to understand which languages your team codes in most
- **MCP Tool Adoption** — Track which MCP servers and tools your team integrates with, including tool_name, mcp_server_name, and usage per day
- **Command Adoption** — See which Cursor commands your team uses most, with command_name and usage per day
- **Plan Mode Adoption** — Measure plan mode adoption with model and usage per day to understand how your team plans before coding
- **Skills Adoption** — Track which Cursor skills your team leverages with skill_name and usage per day
- **Ask Mode Adoption** — Monitor ask mode usage with model and usage per day to see how your team asks questions about their codebase
- **Team Leaderboard** — Rank team members by AI usage metrics with configurable sorting metric, pagination, date range filters, and user filtering

### How it works

1. Subscribe to this server
2. Enter your Cursor Analytics API key (requires admin:* scope, Enterprise teams only)
3. Start querying team analytics from Claude, Cursor, or any MCP-compatible client

Your AI acts as a gateway to Cursor's team analytics — pull usage insights, track adoption trends, and identify top contributors without navigating dashboards.

### Who is this for?

- **Engineering Managers** — track AI coding adoption and measure ROI across the team
- **Team Leads** — identify top contributors and understand which AI features drive productivity
- **Platform Teams** — monitor MCP tool adoption and plan upgrade rollouts based on client version distribution
- **DevOps** — track DAU trends and identify which AI models your team prefers for cost optimization


## Available Tools (12)
- **get_agent_edits**: Supports date range filters and optional user filtering by comma-separated emails or IDs. Date shortcuts: 7d, 30d, today, yesterday, now, ISO 8601, YYYY-MM-DD, or Unix timestamps.

Get AI-suggested code edit metrics for your team
- **get_plans_adoption**: Plan mode lets Cursor plan before coding — useful for tracking adoption of this workflow. Supports date range filters and optional user filtering. Date shortcuts: 7d, 30d, today, yesterday, now, ISO 8601, YYYY-MM-DD, or Unix timestamps.

Get plan mode adoption metrics for your team
- **get_ask_mode_adoption**: Ask mode lets users ask questions about their codebase — useful for tracking this workflow. Supports date range filters and optional user filtering. Date shortcuts: 7d, 30d, today, yesterday, now, ISO 8601, YYYY-MM-DD, or Unix timestamps.

Get ask mode adoption metrics for your team
- **get_client_versions**: Useful for tracking upgrade adoption and identifying outdated installations. Supports date range filters and optional user filtering. Date shortcuts: 7d, 30d, today, yesterday, now, ISO 8601, YYYY-MM-DD, or Unix timestamps.

Get the distribution of Cursor client versions across your team
- **get_commands_adoption**: Useful for understanding which Cursor commands your team uses most. Supports date range filters and optional user filtering. Date shortcuts: 7d, 30d, today, yesterday, now, ISO 8601, YYYY-MM-DD, or Unix timestamps.

Get Cursor command adoption metrics for your team
- **get_daily_active_users**: Supports date range filters and optional user filtering. Date shortcuts: 7d, 30d, today, yesterday, now, ISO 8601, YYYY-MM-DD, or Unix timestamps.

Get daily active user counts for your team
- **get_leaderboard**: Supports sorting by metric (default combinedLinesAccepted), pagination with page and pageSize, date range filters, and optional user filtering. Available metrics: combinedLinesAccepted, combinedLinesSuggested, tabAccepts, agentEditsAccepted, messages, and more. Date shortcuts: 7d, 30d, today, yesterday, now, ISO 8601, YYYY-MM-DD, or Unix timestamps.

Get the team leaderboard ranked by AI usage metrics
- **get_mcp_adoption**: Useful for understanding which MCP servers and tools your team integrates most. Supports date range filters and optional user filtering. Date shortcuts: 7d, 30d, today, yesterday, now, ISO 8601, YYYY-MM-DD, or Unix timestamps.

Get MCP tool adoption metrics for your team
- **get_model_usage**: Useful for understanding which AI models your team prefers. Supports date range filters and optional user filtering. Date shortcuts: 7d, 30d, today, yesterday, now, ISO 8601, YYYY-MM-DD, or Unix timestamps.

Get AI model usage breakdown for your team
- **get_skills_adoption**: Useful for understanding which Cursor skills your team leverages most. Supports date range filters and optional user filtering. Date shortcuts: 7d, 30d, today, yesterday, now, ISO 8601, YYYY-MM-DD, or Unix timestamps.

Get skills adoption metrics for your team
- **get_tab_usage**: Supports date range filters and optional user filtering. Date shortcuts: 7d, 30d, today, yesterday, now, ISO 8601, YYYY-MM-DD, or Unix timestamps.

Get tab autocomplete usage metrics for your team
- **get_top_file_extensions**: Useful for understanding which languages your team codes in most. Supports date range filters and optional user filtering. Date shortcuts: 7d, 30d, today, yesterday, now, ISO 8601, YYYY-MM-DD, or Unix timestamps.

Get the top 5 file extensions per day by suggestion volume


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cursor Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the daily active users for the last 14 days."

**🤖 AI Agent:**
> Retrieving DAU data for the last 14 days... Here's the trend: DAU peaked at 48 on July 3rd and averaged 35 across the period. CLI usage was consistent at 10-12 daily active users, cloud agent usage grew from 3 to 8, and Bugbot usage remained steady at 2-3. Would you like to see the breakdown by user?

---

**👤 You:**
> "What AI models are most used by my team?"

**🤖 AI Agent:**
> Fetching model usage data... Over the last 7 days, claude-sonnet-4 led with 4,200 messages from 12 users, followed by gpt-4 with 1,800 messages from 8 users, and gemini-2.5-pro with 900 messages from 5 users. Claude Sonnet 4 accounts for 60% of all AI interactions. Would you like to see the daily breakdown or filter by specific users?

---

**👤 You:**
> "Show the agent edit acceptance rate for the last 30 days."

**🤖 AI Agent:**
> Retrieving agent edit metrics... Over the last 30 days, your team received 15,000 suggested diffs and accepted 9,200, for an overall acceptance rate of 61%. The team also accepted 28,500 of 42,000 suggested lines (68% line acceptance rate). Acceptance rates have been trending upward — from 55% in week one to 67% in week four. Would you like the leaderboard to see who's accepting the most?


## ❓ FAQ

**Q: How do I get a Cursor Analytics API key?**
Sign in to your Cursor Dashboard, navigate to Settings → API Keys, and generate a new API key. Ensure the key has the `admin:*` scope — Analytics API access requires it. The key format is `crsr_xxx`. Copy it immediately as it may not be shown again. Paste it into the API key field above to connect.

**Q: Is an Enterprise plan required to use the Analytics API?**
Yes. The Cursor Analytics API is available exclusively to Enterprise teams. If your team is not on an Enterprise plan, API requests will return HTTP 403 Forbidden. Contact your Cursor account manager or upgrade to Enterprise to gain access.

**Q: What analytics metrics are available?**
This MCP provides 12 analytics endpoints: agent edits (suggested/accepted/rejected diffs and lines), tab autocomplete usage (suggestions, accepts, rejects, lines), daily active users (with CLI, cloud agent, and bugbot breakdowns), client version distribution, AI model usage (messages and users per model per day), top 5 file extensions per day, MCP tool adoption, Cursor command adoption, plan mode adoption, skills adoption, ask mode adoption, and a team leaderboard with configurable sorting and pagination.

**Q: What date formats does the API support?**
All analytics endpoints support the following date formats for startDate and endDate: relative shortcuts (`7d`, `30d`, `today`, `yesterday`, `now`), ISO 8601 strings (e.g. `2026-07-10T00:00:00Z`), calendar dates in `YYYY-MM-DD` format, and Unix timestamps. When omitted, startDate defaults to `7d` and endDate defaults to `today`.

**Q: Can I filter analytics by specific users?**
Yes. All analytics endpoints accept an optional `users` parameter with comma-separated email addresses or user IDs. When provided, the API returns metrics filtered to only those users. This is useful for tracking individual or subgroup performance, or comparing team members on the leaderboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cursor-analytics](https://vinkius.com/mcp/cursor-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cursor Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cursor-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cursor Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cursor-analytics": {
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
