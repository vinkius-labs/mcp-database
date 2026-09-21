# Offside Line Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/offside-line-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Determines football offside status and margins using defender and ball coordinates.

## Description
This MCP server provides precise tools for calculating offside positions in football. By analyzing the X and Y coordinates of the attacking player, the ball, and the defenders, it applies the second-last opponent rule to determine the offside line. It can identify if a player is onside or offside and calculate the exact margin in meters. Use `get_offside_status` to find the status and margin, `validate_pitch_coordinates` to ensure data integrity, `get_defender_proximity` to check defensive gaps, and `get_reference_line_type` to see if the goal line or a defender defines the line.


## Available Tools (4)
- **get_defender_proximity**: Calculates proximity to defenders
- **get_offside_status**: 
- **get_reference_line_type**: Identifies reference line type
- **validate_pitch_coordinates**: Validates pitch boundaries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Offside Line Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the attacker at (85, 34) offside? The ball is at (80, 34), the goal line is at 105, and defenders are at (90, 30) and (95, 35)."

**🤖 AI Agent:**
> No, the attacker is onside because they are behind the ball.

---

**👤 You:**
> "Calculate the offside status for an attacker at (92, 34) when the ball is at (80, 34) and defenders are at (95, 30) and (98, 35). The goal line is at 105."

**🤖 AI Agent:**
> The attacker is offside with a margin of 3 meters from the reference line.

---

**👤 You:**
> "Check if the coordinates (110, 40) are valid for a standard pitch of 105x68."

**🤖 AI Agent:**
> The coordinates are invalid because the X-coordinate exceeds the pitch length.


## ❓ FAQ

**Q: How is the offside line determined?**
The offside line is defined by the second-to-last opponent. If there are fewer than two opponents between the attacker and the goal, the goal line itself becomes the reference line.

**Q: Does the ball position affect the offside decision?**
Yes. If the attacking player is behind the ball at the moment of the pass, they are considered onside regardless of the defenders' positions.

**Q: What happens if a player is perfectly level with the defender?**
If an attacker is perfectly level with the reference line or the ball, they are considered onside.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/offside-line-calculator](https://vinkius.com/en/ai-agent-connect/offside-line-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Offside Line Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `offside-line-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Offside Line Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "offside-line-calculator": {
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
