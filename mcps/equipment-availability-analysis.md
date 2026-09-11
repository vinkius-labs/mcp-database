# Equipment Availability Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/equipment-availability-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Quantify industrial equipment performance using availability, utilization, and OEE metrics.

## Description
This MCP server provides specialized tools for industrial performance analysis. It allows AI agents to calculate critical manufacturing metrics including Availability, Utilization, and Overall Equipment Effectiveness (OEE). By processing operating hours, planned downtime, and unplanned downtime, the server helps identify production losses and equipment reliability. Use `calculate_availability` to check reliability, `calculate_utilization` to measure capacity usage, `calculate_oee` for total effectiveness, and `summarize_downtime_impact` to assess schedule disruptions.


## Available Tools (4)
- **calculate_availability**: Calculate equipment availability
- **calculate_oee**: Calculate Overall Equipment Effectiveness (OEE)
- **calculate_utilization**: Calculate equipment utilization
- **summarize_downtime_impact**: Summarize downtime impact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Equipment Availability Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the OEE if availability is 0.9, performance is 0.85, and quality is 0.98."

**🤖 AI Agent:**
> The Overall Equipment Effectiveness (OEE) is 74.97%.

---

**👤 You:**
> "The machine was scheduled for 480 minutes. There was 30 minutes of unplanned downtime. What is the availability?"

**🤖 AI Agent:**
> The equipment availability is 93.75%.

---

**👤 You:**
> "Summarize the downtime impact for a 1000 minute shift with 50 minutes of planned downtime and 20 minutes of unplanned downtime."

**🤖 AI Agent:**
> The planned downtime ratio is 5%, the unplanned downtime ratio is 2%, and the total loss ratio is 7%.


## ❓ FAQ

**Q: How do I calculate the total effectiveness of my machine?**
You can use the `calculate_oee` tool. Provide the availability, performance rate, and quality rate as decimals between 0 and 1 to get the total OEE percentage.

**Q: What is the difference between planned and unplanned downtime in these calculations?**
Planned downtime refers to scheduled stops like maintenance, while unplanned downtime refers to unexpected failures. The `summarize_downtime_impact` tool helps distinguish how each affects your production schedule.

**Q: Can I use this to check if my equipment is reliable?**
Yes, use the `calculate_availability` tool with your scheduled time and unplanned downtime to determine the reliability of your equipment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/equipment-availability-analysis](https://vinkius.com/en/ai-agent-connect/equipment-availability-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Equipment Availability Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `equipment-availability-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Equipment Availability Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "equipment-availability-analysis": {
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
