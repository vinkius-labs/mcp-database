# Vessel Design Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/vessel-design-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Professional ASME-compliant pressure vessel dimension and structural requirement calculator.

## Description
This MCP server provides essential engineering tools for designing pressure vessels according to the ASME Boiler and Pressure Vessel Code. It allows AI agents to perform critical structural calculations, including determining the `calculate_shell_thickness` for cylindrical sections, calculating `calculate_head_thickness` for various head geometries, and evaluating `calculate_nozzle_reinforcement` requirements for openings. Users can also retrieve material-specific allowable stress values using `get_material_properties` to ensure design integrity under specific operating temperatures and pressures.


## Available Tools (4)
- **calculate_nozzle_reinforcement**: Determines if an opening in the vessel requires additional reinforcement and calculates the required area
- **calculate_head_thickness**: Calculates the required thickness for the vessel's end caps (heads)
- **calculate_shell_thickness**: Determines the required total wall thickness for the cylindrical portion of the vessel
- **get_material_properties**: Retrieves allowable stress values for specific materials at given temperatures


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vessel Design Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the shell thickness for a vessel with 500 PSI pressure, 400F temperature, 48 inch diameter, SA-516 Grade 70 material, 0.85 joint efficiency, and 0.125 inch corrosion allowance."

**🤖 AI Agent:**
> The required total wall thickness for the shell is 0.625 inches.

---

**👤 You:**
> "What is the allowable stress for SA-516 Grade 70 at 300 degrees Fahrenheit?"

**🤖 AI Agent:**
> The allowable stress for SA-516 Grade 70 at 300°F is 26,000 PSI.

---

**👤 You:**
> "Check if a 4-inch nozzle requires reinforcement on a shell that is 0.5 inches thick with an opening area of 12.57 square inches and a required reinforcement area of 5.0 square inches."

**🤖 AI Agent:**
> No, additional reinforcement is not required for this nozzle configuration.


## ❓ FAQ

**Q: Which engineering standards does this tool follow?**
The calculations are based on the ASME Boiler and Pressure Vessel Code.

**Q: Can I calculate the thickness for different head types?**
Yes, the tool supports hemispherical, ellipsoidal, and torispherical head geometries.

**Q: How does the tool handle corrosion?**
The tool incorporates a corrosion allowance into the total thickness calculations to ensure long-term structural integrity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/vessel-design-calculator](https://vinkius.com/ai-agent-connect/vessel-design-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vessel Design Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vessel-design-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vessel Design Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vessel-design-calculator": {
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
