# HVAC Load Calculator (Manual J) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hvac-load-calculator-manual-j)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate heating and cooling loads in BTU/h and Tons using simplified Manual J standards.

## Description
This MCP server provides a simplified thermal load calculation engine based on the Manual J standard. It allows HVAC professionals and engineers to determine the precise heating and cooling requirements for residential spaces. By using tools like `calculate_heating_demand`, `calculate_cooling_demand`, and `validate_equipment_capacity`, you can calculate heat loss through building envelopes, solar gain from window orientations, and internal heat gains from occupancy. The server also enables checking if a specific HVAC unit's rated capacity is sufficient for the calculated loads.


## Available Tools (3)
- **calculate_cooling_demand**: Calculates the cooling load in BTU/h and Tons
- **calculate_heating_demand**: Calculates the heating load in BTU/h
- **validate_equipment_capacity**: Evaluates if an HVAC unit capacity is sufficient


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HVAC Load Calculator (Manual J)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the heating demand for a 2000 sq ft space with medium insulation in climate zone 5."

**🤖 AI Agent:**
> The calculated heating load is 45,000 BTU/h.

---

**👤 You:**
> "What is the cooling load for a 1500 sq ft room with north: 50, south: 20, east: 10, west: 10 window areas and 3 people?"

**🤖 AI Agent:**
> The cooling load is 18,500 BTU/h (approximately 1.54 Tons).

---

**👤 You:**
> "Is a 24,000 BTU unit enough for a load of 20,000 BTU heating and 26,000 BTU cooling?"

**🤖 AI Agent:**
> No, the unit is Underpowered because it does not meet the required cooling load.


## ❓ FAQ

**Q: What does the `calculate_heating_demand` tool do?**
It determines the total heating capacity required (in BTU/h) by considering the conditioned area, insulation level, and IECC climate zone.

**Q: How can I check if my HVAC unit is large enough?**
Use the `validate_equipment_capacity` tool by providing the required heating load, required cooling load, and the nominal BTU capacity of your unit.

**Q: Does the cooling calculation include solar gain?**
Yes, the `calculate_cooling_demand` tool accounts for solar radiation through window areas in all four cardinal directions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hvac-load-calculator-manual-j](https://vinkius.com/mcp/hvac-load-calculator-manual-j)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HVAC Load Calculator (Manual J)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hvac-load-calculator-manual-j` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HVAC Load Calculator (Manual J)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hvac-load-calculator-manual-j": {
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
