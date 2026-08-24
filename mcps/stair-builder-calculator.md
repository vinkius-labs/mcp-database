# Stair Builder Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/stair-builder-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Deterministic stair design tool for IRC/IBC building code compliance.

## Description
This MCP server provides precise stair design calculations based on strict building codes like IRC and IBC. Use `calculate_stair_geometry` to determine riser heights, tread depths, and total run lengths. You can also use `check_clearance_and_headroom` to ensure vertical safety and `validate_landing_requirements` to confirm if your staircase layout needs a landing. It flags code violations automatically to ensure safe and ergonomic stair construction.


## Available Tools (3)
- **check_clearance_and_headroom**: Validates vertical headroom clearance
- **calculate_stair_geometry**: Calculates primary stair dimensions and structural requirements
- **validate_landing_requirements**: Determines if the staircase layout complies with landing requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stair Builder Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the dimensions for a straight staircase with a total rise of 100 inches and a desired tread depth of 11 inches."

**🤖 AI Agent:**
> For a 100-inch rise and 11-inch tread, you will have 14 risers at 7.14 inches each. The total run will be 132 inches.

---

**👤 You:**
> "Will my stairs have enough headroom if the ceiling height is 80 inches?"

**🤖 AI Agent:**
> No, the headroom clearance is below the required 6'8" (80 inches) minimum standard.

---

**👤 You:**
> "Do I need a landing for a straight staircase with a total run of 15 feet?"

**🤖 AI Agent:**
> Yes, a landing is required because the total run exceeds the 12-foot limit for straight stairs.


## ❓ FAQ

**Q: How does the tool ensure building code compliance?**
The tool uses `calculate_stair_geometry` to check dimensions against IRC/IBC limits, such as maximum riser height and the stride rule.

**Q: Can I check if my stairs have enough headroom?**
Yes, by using the `check_clearance_and_headroom` tool, you can validate vertical clearance against the minimum 6'8" requirement.

**Q: What stair types are supported?**
The calculator supports straight, l_shaped, u_shaped, and spiral stair configurations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/stair-builder-calculator](https://vinkius.com/ai-agent-connect/stair-builder-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stair Builder Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stair-builder-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stair Builder Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stair-builder-calculator": {
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
