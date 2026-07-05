# Room Layout Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/room-layout-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [interior-design](../categories/interior-design.md)

Checks if furniture fits in a room by evaluating placement integrity, walkability, and clearance compliance.

## Description
The Room Layout Planner MCP server provides essential tools for spatial analysis of interior layouts. It allows you to verify if furniture placement is feasible by using `validate_placement_integrity` to check for boundary violations and obstructions like doors or windows. You can assess the usability of a space with `calculate_walkability_score`, which measures the proportion of unobstructed floor area. Additionally, `check_clearance_compliance` identifies narrow walkways or insufficient ergonomic gaps between items, such as the required distance between a sofa and a coffee table.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Room Layout Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is my sofa placement valid?"

**🤖 AI Agent:**
> Yes, the sofa is within boundaries and does not block any windows.

---

**👤 You:**
> "Calculate the walkability of this room."

**🤖 AI Agent:**
> The total room area is 144 sq ft, with an occupied area of 40 sq ft, resulting in a walkability score of 72.2%.

---

**👤 You:**
> "Are there any clearance issues?"

**🤖 AI Agent:**
> Yes, the gap between the sofa and coffee table is only 12 inches, which is below the required 18-inch threshold.


## ❓ FAQ

**Q: How does the tool check for obstructions?**
The `validate_placement_integrity` tool checks if any furniture pieces overlap with defined obstruction zones like doors and windows. Tools available: `your_tool_name`.

**Q: What does the walkability score represent?**
The walkability score is a percentage representing the ratio of unoccupied floor area to the total room area.

**Q: Does it check for ergonomic spacing?**
Yes, `check_clearance_compliance` identifies if gaps between furniture pieces are too narrow for walkways or seating comfort.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/room-layout-planner](https://vinkius.com/mcp/room-layout-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Room Layout Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `room-layout-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Room Layout Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "room-layout-planner": {
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
