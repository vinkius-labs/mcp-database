# Lineup Priority Logic Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/lineup-priority-logic-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [safety](../categories/safety.md)

Deterministic surfing right-of-way and priority violation validator.

## Description
This MCP server provides precise tools for determining surfing right-of-way and identifying priority violations. It calculates priority scores based on distance to the peak, surfer position (inside vs. outside), and current state (standing vs. paddling). Use `calculate_lineup_priority` to rank surfers and identify drop-in violations, `validate_position_legality` to ensure surfer positions match wave behavior, and `get_lineup_summary` for a high-level overview of lineup density.


## Available Tools (3)
- **calculate_lineup_priority**: Determines the priority ranking and right-of-way status for a group of surfers in a specific wave scenario
- **validate_position_legality**: Checks if the current surfer positions relative to the wave direction are physically consistent with the wave's behavior
- **get_lineup_summary**: Provides a high-level overview of the current lineup density and priority distribution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lineup Priority Logic Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the priority for these surfers: surfer_1 (10m from peak, inside, standing), surfer_2 (5m from peak, outside, paddling) with a left breaking wave."

**🤖 AI Agent:**
> The priority scores are: surfer_1: 140, surfer_2: 95. The right-of-way holder is surfer_1.

---

**👤 You:**
> "Is there a drop-in violation if surfer_2 (score 40) takes a wave when surfer_1 (score 80) has the right of way?"

**🤖 AI Agent:**
> Yes, a drop-in violation is flagged because the score difference is 40, which exceeds the 20-point threshold.

---

**👤 You:**
> "Give me a summary of the lineup: surfer_1 (inside), surfer_2 (outside), surfer_3 (inside)."

**🤖 AI Agent:**
> The lineup contains 3 surfers, with 2 surfers inside and 1 surfer outside.


## ❓ FAQ

**Q: How is priority calculated?**
Priority is calculated using a base score from distance to the peak, with significant boosts for being 'inside' the pocket or already standing on the board.

**Q: What constitutes a drop-in violation?**
A violation is flagged if a surfer takes a wave when their priority score is more than 20 points lower than the right-of-way holder.

**Q: Can I check if my lineup configuration is valid?**
Yes, you can use the `validate_position_legality` tool to ensure surfer positions are physically consistent with the wave direction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/lineup-priority-logic-validator](https://vinkius.com/ai-agent-connect/lineup-priority-logic-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lineup Priority Logic Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lineup-priority-logic-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lineup Priority Logic Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lineup-priority-logic-validator": {
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
