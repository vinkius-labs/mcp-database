# Kayak Distance & Session Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/kayak-distance-session-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate total distance, average speed, and session summaries for paddling activities.

## Description
This MCP server provides tools to manage and analyze kayaking data. It allows you to calculate the total distance traveled using `get_total_distance`, determine your average speed with `get_average_speed`, validate the integrity of your paddling logs via `validate_segment_data`, and generate comprehensive session overviews using `summarize_paddling_session`.


## Available Tools (4)
- **summarize_paddling_session**: Provides a high-level overview of a paddling session
- **get_average_speed**: Determines the average speed of travel across a series of segments
- **get_total_distance**: Calculates the total distance traveled across all provided paddling segments
- **validate_segment_data**: Checks if a provided set of paddling segments follows the required format and physical constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kayak Distance & Session Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total distance for these segments: 5km, 10km, and 2mi?"

**🤖 AI Agent:**
> The total distance is 17.22 kilometers.

---

**👤 You:**
> "Calculate my average speed for a 10km segment that took 30 minutes."

**🤖 AI Agent:**
> Your average speed was 20.0 km/h.

---

**👤 You:**
> "Summarize this session: 5km in 20 mins and 5mi in 40 mins."

**🤖 AI Agent:**
> The session summary is: Total distance is 13.09 km, total duration is 60 minutes, and average speed is 13.09 km/h.


## ❓ FAQ

**Q: How do I calculate my total distance?**
You can use the `get_total_distance` tool by providing an array of segments, each containing a distance and a unit (km or mi).

**Q: Can I mix kilometers and miles in my data?**
Yes, the tools automatically handle unit conversion to ensure accurate calculations across mixed-unit logs.

**Q: How can I check if my paddling data is valid?**
Use the `validate_segment_data` tool to check if your segments follow the required format and physical constraints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/kayak-distance-session-tracker](https://vinkius.com/en/ai-agent-connect/kayak-distance-session-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kayak Distance & Session Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kayak-distance-session-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kayak Distance & Session Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kayak-distance-session-tracker": {
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
