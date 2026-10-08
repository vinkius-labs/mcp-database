# Meeting Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/meeting-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate the economic impact of meetings by aggregating attendee compensation, duration, and preparation time.

## Description
This MCP server provides tools to quantify the hidden costs of synchronous collaboration. Use `summarize_meeting_series` to get a full report on per-meeting and annual costs, or `get_meeting_efficiency_score` to evaluate if a meeting's importance justifies its financial impact. It accounts for attendee compensation, meeting duration, and the critical preparation time required for each participant.


## Available Tools (4)
- **calculate_annual_impact**: Projects the total cost of a recurring meeting series over a full year
- **calculate_single_meeting_cost**: Calculates the total labor cost for one single instance of a meeting
- **get_meeting_efficiency_score**: Provides a ratio to help determine if the meeting's purpose justifies its cost
- **summarize_meeting_series**: Aggregates all meeting metrics into a single report for a specific series


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meeting Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost for a 1-hour meeting with three people earning $50, $60, and $70 per hour, including 0.5 hours of prep time each?"

**🤖 AI Agent:**
> The total cost for this single meeting is $270.00, with a total of 4.5 labor hours spent.

---

**👤 You:**
> "Calculate the annual cost of a monthly meeting that costs $400 per instance."

**🤖 AI Agent:**
> The total annual cost for this meeting series is $4,800.00.

---

**👤 You:**
> "Is a meeting costing $500 with 5 attendees and a decision weight of 1000 efficient?"

**🤖 AI Agent:**
> Yes, with a score of 2.0, this meeting is rated as High Efficiency.


## ❓ FAQ

**Q: How does the tool account for preparation time?**
The `summarize_meeting_series` tool includes the preparation time for every attendee in both the per-meeting and annual cost calculations.

**Q: Can I calculate the yearly impact of a weekly meeting?**
Yes, you can use `calculate_annual_impact` by providing the per-meeting cost and a frequency of 52 for a weekly meeting.

**Q: What is an efficiency score?**
The efficiency score, calculated via `get_meeting_efficiency_score`, is a ratio of the meeting's decision weight to its total cost, helping you determine if the meeting is worth the investment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/meeting-cost-calculator](https://vinkius.com/en/ai-agent-connect/meeting-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Meeting Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `meeting-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Meeting Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meeting-cost-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
