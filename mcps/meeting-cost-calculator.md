# Meeting Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/meeting-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Quantify the financial impact of corporate meetings.

## Description
This MCP server provides tools to calculate the economic cost of meetings. Use `calculate_single_meeting_cost` to find the total expenditure for a specific session, or `estimate_meeting_efficiency` to check if a meeting stays within a defined budget. You can also use `batch_calculate_meeting_costs` to compare multiple scenarios or `find_optimal_attendee_count` to determine the maximum number of participants allowed under a specific budget limit.


## Available Tools (4)
- **batch_calculate_meeting_costs**: Calculates costs for a list of different meeting scenarios to compare them
- **calculate_single_meeting_cost**: Calculates the total financial cost for a single specific meeting
- **estimate_meeting_efficiency**: Evaluates if a meeting's cost is justified relative to a defined budget threshold
- **find_optimal_attendee_count**: Determines how many attendees can be present without exceeding a specific budget


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meeting Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the cost of a 60-minute meeting with 10 people earning $50 per hour?"

**🤖 AI Agent:**
> The total cost for this meeting is $500.00, with a cost of $50.00 per attendee.

---

**👤 You:**
> "How many people can attend a 30-minute meeting if the average rate is $100/hr and my budget is $250?"

**🤖 AI Agent:**
> You can have a maximum of 5 attendees for this meeting.

---

**👤 You:**
> "Is a 45-minute meeting with 5 people at $60/hr within a $150 budget?"

**🤖 AI Agent:**
> Yes, the meeting is within budget. The total cost is $75.00.


## ❓ FAQ

**Q: How is the meeting cost calculated?**
The cost is calculated by multiplying the number of attendees by the meeting duration (in hours) and the average hourly rate of the participants.

**Q: Can I compare multiple meeting scenarios at once?**
Yes, you can use the `batch_calculate_meeting_costs` tool to process a list of different meeting configurations simultaneously.

**Q: How do I know if my meeting is over budget?**
You can use `estimate_meeting_efficiency` to compare the calculated cost against your specific budget limit.


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
