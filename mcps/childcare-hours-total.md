# Childcare Hours Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/childcare-hours-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Aggregates and analyzes childcare duration data, including overlap detection and provider summaries.

## Description
This MCP server provides tools to manage and analyze childcare duration data. It allows for calculating the total unique time a child is under care using `calculate_total_care_hours`, which accounts for overlapping sessions. Users can also use `identify_overlap_conflicts` to detect scheduling overlaps, `summarize_care_by_provider` to see hours per provider, and `get_care_tier_status` to classify care intensity (e.g., Part-time or Full-time). It acts as a bridge between childcare scheduling data and AI agents in Cursor, VS Code, Claude Desktop, and Windsurf.


## Available Tools (4)
- **summarize_care_by_provider**: Aggregates the total hours provided by each distinct childcare provider
- **calculate_total_care_hours**: Calculates the total unique time a child was under care
- **get_care_tier_status**: Determines the care classification (e.g., Part-time, Full-time) based on total hours
- **identify_overlap_conflicts**: Detects if any provided childcare sessions overlap in time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Childcare Hours Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total unique care hours for these sessions in America/New_York: [{start: '2024-06-01T08:00:00', end: '2024-06-01T12:00:00'}, {start: '2024-06-01T10:00:00', end: '2024-06-01T14:00:00'}]"

**🤖 AI Agent:**
> The total unique care hours provided is 6.0 hours.

---

**👤 You:**
> "Are there any overlapping sessions in this list: [{id: '1', start: '2024-06-01T09:00:00', end: '2024-06-01T11:00:00'}, {id: '2', start: '2024-06-01T10:30:00', end: '2024-06-01T12:00:00'}]?"

**🤖 AI Agent:**
> Yes, there is an overlap between session 1 and session 2.

---

**👤 You:**
> "What is the care tier status for 45 total hours?"

**🤖 AI Agent:**
> The care tier is Full-time.


## ❓ FAQ

**Q: How does the tool handle overlapping childcare sessions?**
The `calculate_total_care_hours` tool calculates the union of all time intervals. This ensures that if two sessions overlap, the overlapping period is only counted once toward the total hours.

**Q: Can I see how many hours each provider worked?**
Yes, you can use the `summarize_care_by_provider` tool to get a list of total hours worked by each distinct provider ID.

**Q: What are the care tiers?**
Care tiers (such as Part-time or Full-time) are determined by the total hours provided, which can be checked using the `get_care_tier_status` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/childcare-hours-total](https://vinkius.com/en/ai-agent-connect/childcare-hours-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Childcare Hours Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `childcare-hours-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Childcare Hours Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "childcare-hours-total": {
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
