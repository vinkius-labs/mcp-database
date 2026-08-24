# HVAC Load Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/hvac-load-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate residential heating and cooling loads using simplified Manual J principles.

## Description
This MCP server provides precise thermal load estimations for residential spaces. By analyzing room dimensions, insulation quality, window orientation, and climate zones, it calculates the necessary BTU/h for both heating and cooling. Use `validate_room_configuration` to ensure your inputs are consistent, then use `get_cooling_load` or `get_heating_load` to determine the required capacity for your HVAC system.


## Available Tools (3)
- **get_cooling_load**: Calculates the total cooling capacity required to maintain temperature in a residential room
- **get_heating_load**: Calculates the total heating capacity required to maintain temperature in a residential room
- **validate_room_configuration**: Validates if the provided room dimensions and environmental factors are physically and logically consistent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HVAC Load Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the cooling load for a 20x20x10 room with average insulation, 2 windows facing South, and 3 occupants."

**🤖 AI Agent:**
> The required cooling capacity for this room is 10,400 BTU/h.

---

**👤 You:**
> "What is the heating load for a 15x15x8 room with good insulation in climate zone 5 and 1 occupant?"

**🤖 AI Agent:**
> The required heating capacity for this room is 12,500 BTU/h.

---

**👤 You:**
> "Check if my room configuration is valid: 12ft length, 12ft width, 8ft height, and 3 windows."

**🤖 AI Agent:**
> The room configuration is valid.


## ❓ FAQ

**Q: How accurate are these calculations?**
The calculations use simplified Manual J principles to provide reliable residential estimates based on standard thermal resistance and climate zone data.

**Q: What is the purpose of the validation tool?**
The `validate_room_configuration` tool ensures that your room dimensions and window counts are logically consistent before you perform any load calculations.

**Q: Can I account for different insulation qualities?**
Yes, you can specify insulation as poor, average, or good to adjust the thermal load requirements accordingly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/hvac-load-calculator](https://vinkius.com/ai-agent-connect/hvac-load-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HVAC Load Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hvac-load-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HVAC Load Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hvac-load-calculator": {
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
