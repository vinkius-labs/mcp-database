# Storage Tank Design (API 650) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/storage-tank-design-api-650)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design atmospheric storage tanks following API 650 standards.

## Description
This MCP server provides engineering tools to design atmospheric storage tanks according to the API 650 standard. It allows AI agents to calculate critical tank parameters including physical footprint via `get_tank_dimensions`, determine necessary shell thickness with `calculate_shell_thickness`, assess stability against environmental loads using `evaluate_environmental_stability`, and specify roof structures with `design_tank_roof`.


## Available Tools (4)
- **design_tank_roof**: Determines the type and thickness of the roof structure
- **calculate_shell_thickness**: Determines the necessary thickness of the vertical steel plates for the tank shell
- **evaluate_environmental_stability**: Assesses the tank's resistance to wind and seismic forces
- **get_tank_dimensions**: Calculates the physical footprint and height of the tank based on required volume


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Storage Tank Design (API 650)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the dimensions for a tank with a capacity of 5000 cubic meters."

**🤖 AI Agent:**
> The tank will have a diameter of 20 meters and a height of approximately 15.92 meters, with a footprint area of 314.16 square meters.

---

**👤 You:**
> "What is the required shell thickness for a tank with 10m diameter, 15m height, 900 kg/m3 density, and 250 MPa yield strength?"

**🤖 AI Agent:**
> The required shell thickness is 8.5 mm, with a bottom plate thickness of 12.0 mm and a corrosion allowance of 2.0 mm.

---

**👤 You:**
> "Design a fixed roof for a tank with 12m diameter and 5 kPa internal pressure."

**🤖 AI Agent:**
> The design specifies a fixed roof with a thickness of 5.5 mm and requires standard structural support.


## ❓ FAQ

**Q: What standards does this tool follow?**
All calculations and design parameters are based on the API 650 standard for atmospheric storage tanks.

**Q: Can I calculate shell thickness for different materials?**
Yes, by using `calculate_shell_thickness`, you can specify the material yield strength to determine the required thickness.

**Q: Does it account for environmental factors?**
Yes, the `evaluate_environmental_stability` tool assesses resistance to both wind and seismic forces.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/storage-tank-design-api-650](https://vinkius.com/ai-agent-connect/storage-tank-design-api-650)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Storage Tank Design (API 650)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `storage-tank-design-api-650` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Storage Tank Design (API 650)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "storage-tank-design-api-650": {
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
