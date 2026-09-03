# Waterproofing Material Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/waterproofing-material-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate precise waterproofing membrane, adhesive, and reinforcement fabric requirements.

## Description
This MCP server provides specialized tools for construction professionals to estimate waterproofing material needs. It calculates the total membrane area required by accounting for application layers, overlap percentages, and waste factors. Additionally, it estimates the necessary volume of adhesive based on membrane thickness and surface texture, and determines the amount of reinforcement fabric needed for complex geometries. Use `calculate_membrane_requirement` to start your estimation process.


## Available Tools (4)
- **calculate_reinforcement_fabric**: Estimates the linear or square meters of reinforcement fabric required for joints and corners
- **generate_material_summary**: Consolidates all individual material calculations into a single procurement list
- **calculate_membrane_requirement**: Determines the total amount of waterproofing membrane needed for a specific surface area
- **estimate_adhesive_needs**: Calculates the volume of adhesive required based on the membrane area


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Waterproofing Material Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much waterproofing membrane do I need for a 100m² area with 2 layers, 10% overlap, and 5% waste?"

**🤖 AI Agent:**
> For a 100m² area with 2 layers, 10% overlap, and 5% waste, you will need 231.0 m² of membrane.

---

**👤 You:**
> "Calculate the adhesive needed for 200m² of membrane that is 3mm thick on a rough surface (factor 1.5)."

**🤖 AI Agent:**
> The estimated adhesive volume required is 45.0 Liters.

---

**👤 You:**
> "Give me a full material summary for 150m² membrane, 20L adhesive, and 10m² fabric."

**🤖 AI Agent:**
> The procurement summary is: 150.0 m² of membrane, 20.0 L of adhesive, and 10.0 m² of reinforcement fabric.


## ❓ FAQ

**Q: How does the tool account for material waste?**
The `calculate_membrane_requirement` tool includes a waste factor parameter, which allows you to add a specific percentage of extra material to cover cutting, scraps, and site-specific losses.

**Q: Can I estimate adhesive needs for different membrane thicknesses?**
Yes, the `estimate_adhesive_needs` tool calculates adhesive volume by considering the total membrane area, the specific thickness of the membrane, and the surface texture of the substrate.

**Q: How is reinforcement fabric calculated?**
Reinforcement fabric requirements are determined using `calculate_reinforcement_fabric`, which uses the application area and a complexity score to estimate the material needed for joints and corners.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/waterproofing-material-calculator](https://vinkius.com/ai-agent-connect/waterproofing-material-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Waterproofing Material Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `waterproofing-material-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Waterproofing Material Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "waterproofing-material-calculator": {
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
