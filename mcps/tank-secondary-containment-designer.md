# Tank Secondary Containment Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tank-secondary-containment-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Automated design for storage tank containment systems, including volume, dimensions, and liners.

## Description
This MCP server provides specialized engineering tools for designing secondary containment systems for storage tanks. It automates the calculation of required containment volumes by accounting for the largest tank capacity alongside firewater and rainwater allowances. Users can use `design_bund_dimensions` to determine physical footprints, `assess_liner_requirements` to calculate necessary material coverage, and `design_drainage_system` to specify water management protocols. It ensures safety compliance by integrating regulatory considerations into the design process.


## Available Tools (4)
- **assess_liner_requirements**: Determines the necessary surface area and material coverage for the containment
- **calculate_containment_volume**: Determines the total required volume for a containment area
- **design_bund_dimensions**: Calculates the physical dimensions of the dike/bund
- **design_drainage_system**: Defines the specifications for the water management system


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tank Secondary Containment Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the required volume for three tanks with capacities of 500, 1200, and 800 cubic meters, with 200 cubic meters for firewater and 50 cubic meters for rain."

**🤖 AI Agent:**
> The total required volume is 1450 cubic meters, with the largest tank capacity being 1200 cubic meters.

---

**👤 You:**
> "What are the dimensions for a rectangular bund that needs to hold 1500 cubic meters, with a maximum height of 3 meters and 600 square meters of available area?"

**🤖 AI Agent:**
> The designed rectangular bund will have a length of 25 meters, a width of 20 meters, and a height of 3 meters, covering a floor area of 500 square meters.

---

**👤 You:**
> "Calculate the liner area for a bund with length 20m, width 15m, and height 2m using concrete."

**🤖 AI Agent:**
> The total liner area required is 460 square meters, consisting of 300 square meters for the floor and 160 square meters for the walls.


## ❓ FAQ

**Q: How is the total containment volume calculated?**
The volume is determined by taking the capacity of the largest single tank and adding the specified allowances for firewater and rainwater.

**Q: Can I design different shapes for the bund?**
Yes, you can specify a preference for rectangular or circular geometries when using the dimensioning tools.

**Q: Does this tool account for liner materials?**
Yes, the `assess_liner_requirements` tool calculates the total surface area needed for both the floor and walls based on the chosen material type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tank-secondary-containment-designer](https://vinkius.com/en/ai-agent-connect/tank-secondary-containment-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tank Secondary Containment Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tank-secondary-containment-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tank Secondary Containment Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tank-secondary-containment-designer": {
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
