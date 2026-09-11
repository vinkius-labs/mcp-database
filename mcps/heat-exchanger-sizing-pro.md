# Heat Exchanger Sizing Pro MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/heat-exchanger-sizing-pro)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate heat transfer area, LMTD, and physical dimensions for shell and tube heat exchangers.

## Description
This MCP server provides specialized engineering tools for sizing shell and tube heat exchangers. It allows AI agents to perform complex thermodynamic calculations including heat duty, Log Mean Temperature Difference (LMTD), and required heat transfer area. Users can determine physical geometry such as shell diameter and tube count using `get_physical_dimensions`. The toolset covers the entire sizing workflow from initial thermal energy calculation with `get_heat_duty` to final physical specification.


## Available Tools (4)
- **calculate_lmtd**: Determine the Log Mean Temperature Difference (LMTD)
- **get_heat_duty**: Calculate the total thermal energy transferred between fluids
- **get_physical_dimensions**: Determine the physical shell diameter and the necessary number of tubes
- **size_heat_exchanger**: Calculate the required heat transfer area and overall heat transfer coefficient


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heat Exchanger Sizing Pro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the heat duty for a hot fluid with a mass flow rate of 5 kg/s, inlet temperature of 100°C, outlet temperature of 60°C, and specific heat of 4.18 kJ/kg·K."

**🤖 AI Agent:**
> The total heat duty is 836 kW.

---

**👤 You:**
> "What is the LMTD for a counter-current flow where hot fluid goes from 100°C to 60°C and cold fluid goes from 20°C to 40°C?"

**🤖 AI Agent:**
> The Log Mean Temperature Difference (LMTD) is 42.48°C.

---

**👤 You:**
> "Determine the shell diameter and tube count for a required area of 15 m2, tube diameter of 0.025 m, tube length of 3 m, and tube pitch of 0.03 m."

**🤖 AI Agent:**
> The required shell diameter is 0.65 m and the necessary tube count is 127.


## ❓ FAQ

**Q: What flow arrangements are supported?**
The server supports both counter-current and co-current flow arrangements for LMTD calculations.

**Q: Can I calculate the physical size of the exchanger?**
Yes, by using the `get_physical_dimensions` tool, you can determine the shell diameter and the required number of tubes.

**Q: How is the heat duty calculated?**
The `get_heat_duty` tool calculates the total thermal energy transferred based on mass flow rate, inlet/outlet temperatures, and specific heat capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/heat-exchanger-sizing-pro](https://vinkius.com/en/ai-agent-connect/heat-exchanger-sizing-pro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Heat Exchanger Sizing Pro** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `heat-exchanger-sizing-pro` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Heat Exchanger Sizing Pro** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "heat-exchanger-sizing-pro": {
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
