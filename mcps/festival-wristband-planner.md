# Festival Wristband Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/festival-wristband-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Calculate precise wristband inventory requirements for festivals.

## Description
This MCP server provides precision inventory planning for event organizers. It calculates the exact number of wristbands needed based on attendee capacity, event duration, and safety buffers. Use `get_procurement_summary` for a complete report or `get_event_scale_category` to determine the event tier. It supports both single-band multi-day models and daily-replacement models.


## Available Tools (4)
- **get_buffered_wristband_requirement**: Calculates the total wristband count including a specified safety margin
- **get_procurement_summary**: Provides a high-level summary for purchasing departments, combining base needs, buffers, and scale
- **get_event_scale_category**: Determines the organizational tier of the event based on the attendee count
- **get_base_wristband_requirement**: Calculates the absolute minimum number of wristbands needed without any safety buffers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Festival Wristband Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many wristbands do I need for a 3-day festival with 5000 attendees if they use one band for the whole duration and I want a 10% buffer?"

**🤖 AI Agent:**
> You will need 5,500 wristbands in total (5,000 base + 500 buffer).

---

**👤 You:**
> "What scale is an event with 10,000 attendees?"

**🤖 AI Agent:**
> An event with 10,000 attendees is categorized as a Large scale event.

---

**👤 You:**
> "Calculate the wristband requirement for a 2-day event with 1000 people, where each day needs a new band and I want a 5% buffer."

**🤖 AI Agent:**
> You will need 2,100 wristbands in total (2,000 base + 100 buffer).


## ❓ FAQ

**Q: How does the multi-day calculation work?**
If you select a single-band model, the tool assumes one wristband covers all days. If not, it calculates a new wristband requirement for every day of the event.

**Q: What is a safety buffer?**
A safety buffer is an extra percentage of inventory added to your base requirement to account for lost or damaged wristbands.

**Q: Can I get a full report for my purchasing department?**
Yes, you can use the `get_procurement_summary` tool to generate a comprehensive breakdown including base counts, buffered totals, and event scale.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/festival-wristband-planner](https://vinkius.com/en/ai-agent-connect/festival-wristband-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Festival Wristband Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `festival-wristband-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Festival Wristband Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "festival-wristband-planner": {
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
