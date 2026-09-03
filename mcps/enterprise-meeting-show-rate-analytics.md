# Enterprise Meeting Show Rate Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-meeting-show-rate-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze meeting attendance, no-show patterns, and engagement quality.

## Description
This MCP server provides deep insights into enterprise meeting efficiency. It allows AI agents to calculate attendance metrics using `get_show_rate_summary`, identify problematic trends with `analyze_no_show_patterns`, evaluate engagement value via `calculate_meeting_quality`, and assess the impact of notification frequency through `evaluate_reminder_effectiveness`.


## Available Tools (4)
- **calculate_meeting_quality**: Evaluates the effectiveness of meetings based on their outcomes
- **evaluate_reminder_effectiveness**: Determines how the frequency of reminders impacts the likelihood of a meeting being held
- **get_show_rate_summary**: Calculates the high-level attendance percentage for a specific subset of meetings
- **analyze_no_show_patterns**: Identifies which combinations of factors are most likely to result in a no-show


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Meeting Show Rate Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current meeting show rate for virtual meetings?"

**🤖 AI Agent:**
> The current show rate for virtual meetings is 78%, with 125 meetings held out of 160 scheduled.

---

**👤 You:**
> "Are there any significant no-show patterns I should know about?"

**🤖 AI Agent:**
> Yes, there is a significant pattern where Outbound leads for In-Person meetings have a no-show rate of 42%.

---

**👤 You:**
> "How effective are our daily reminders for webinar formats?"

**🤖 AI Agent:**
> Daily reminders for webinars result in an 85% show rate, which is higher than the single 24h reminder cadence.


## ❓ FAQ

**Q: How is the show rate calculated?**
The show rate is the total number of held meetings divided by the total number of scheduled meetings, expressed as a percentage.

**Q: Can I filter metrics by meeting type?**
Yes, tools like `get_show_rate_summary` and `calculate_meeting_quality` allow you to filter results by specific meeting formats.

**Q: What determines the meeting quality score?**
The quality score is a weighted metric where outcomes like 'Scheduled Next Step' carry higher weight than 'No Show' or 'Disqualified'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-meeting-show-rate-analytics](https://vinkius.com/ai-agent-connect/enterprise-meeting-show-rate-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Meeting Show Rate Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-meeting-show-rate-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Meeting Show Rate Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-meeting-show-rate-analytics": {
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
