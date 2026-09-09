# Mud Weight Window Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mud-weight-window-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculates safe drilling fluid density ranges based on geomechanical constraints.

## Description
This MCP server provides specialized tools for drilling engineers to determine the safe operational range for drilling fluid density. It calculates the primary window using `calculate_basic_window` by analyzing pore pressure, fracture gradient, and collapse pressure. The server also allows for advanced adjustments, including `apply_thermal_adjustments` for temperature-induced changes and `apply_chemical_adjustments` for chemical reactivity effects. Finally, use `validate_operational_safety` to verify if a specific mud weight is safe for the wellbore.


## Available Tools (4)
- **apply_thermal_adjustments**: Modifies the basic window to account for temperature-induced changes
- **calculate_basic_window**: Determines the primary drilling window based on standard pressure limits
- **validate_operational_safety**: Evaluates if a proposed mud weight is safe within the calculated window
- **apply_chemical_adjustments**: Adjusts the window to account for chemical interactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mud Weight Window Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the basic mud weight window for a pore pressure of 10.5, a fracture gradient of 14.2, and a collapse pressure of 11.0."

**🤖 AI Agent:**
> The minimum mud weight is 11.0, the maximum mud weight is 14.2, and the safe window is 3.2.

---

**👤 You:**
> "Is a mud weight of 12.5 safe for a window with a minimum of 11.0 and a maximum of 14.2?"

**🤖 AI Agent:**
> Yes, the proposed mud weight is safe. The margin to collapse is 1.5 and the margin to fracture is 1.7.

---

**👤 You:**
> "Adjust a window (min 11.0, max 14.2) for a bottom hole temperature of 150 degrees with a coefficient of 0.01."

**🤖 AI Agent:**
> The adjusted minimum mud weight is 12.5, the adjusted maximum mud weight is 12.7, and the adjusted safe window is 0.2.


## ❓ FAQ

**Q: How do I calculate the initial drilling window?**
You can use the `calculate_basic_window` tool by providing the pore pressure, fracture gradient, and collapse pressure.

**Q: Can I account for temperature changes in the wellbore?**
Yes, the `apply_thermal_adjustments` tool allows you to modify the basic window based on bottom hole temperature and a temperature coefficient.

**Q: How can I check if a specific mud weight is safe?**
Use the `validate_operational_safety` tool with your calculated window and the proposed mud weight to receive a safety report.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mud-weight-window-calculator](https://vinkius.com/ai-agent-connect/mud-weight-window-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mud Weight Window Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mud-weight-window-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mud Weight Window Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mud-weight-window-calculator": {
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
