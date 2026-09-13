# Amine Treating Unit Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/amine-treating-unit-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design amine treating units for acid gas removal by calculating equipment dimensions and energy requirements.

## Description
This MCP server provides specialized engineering tools for designing amine treating units used in acid gas removal. It allows AI agents to calculate critical parameters such as the `get_circulation_rate` to ensure sufficient solvent flow, `design_absorber` for column dimensions, and `design_stripper` for regeneration requirements. Additionally, it includes `evaluate_solvent_health` to assess how contaminants like heat stable salts impact solvent capacity and corrosion risk.


## Available Tools (4)
- **get_circulation_rate**: Determines the required amine flow to meet the acid gas removal targets
- **design_stripper**: Calculates the dimensions and requirements for the regeneration column
- **evaluate_solvent_health**: Assesses the impact of contaminants on the design
- **design_absorber**: Calculates the physical dimensions of the absorption column


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amine Treating Unit Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the required amine circulation rate for a gas flow of 1000 m3/h with 5% acid gas concentration using MDEA and a loading of 0.4."

**🤖 AI Agent:**
> The required circulation rate is 125.5 m3/h with a lean loading of 0.1 and a rich loading of 0.4.

---

**👤 You:**
> "What are the dimensions for an absorber using a circulation rate of 125.5 m3/h and a gas flow of 1000 m3/h with MDEA?"

**🤖 AI Agent:**
> The absorber will have a diameter of 1.2 meters, a height of 8.5 meters, and will require 20 trays.

---

**👤 You:**
> "How much reboiler duty is needed for a stripper with a circulation rate of 125.5 m3/h using DEA and 0.01 HSS concentration?"

**🤖 AI Agent:**
> The required reboiler duty is 4.2 MW.


## ❓ FAQ

**Q: What can I calculate with this server?**
You can calculate amine circulation rates, absorber and stripper dimensions, reboiler duty, and evaluate solvent health based on heat stable salt concentrations.

**Q: Does this support selective H2S removal?**
Yes, the `design_absorber` tool includes a parameter to prioritize selective H2S removal during the design process.

**Q: How does HSS affect my design?**
Heat Stable Salts (HSS) reduce the effective capacity of the amine and increase corrosion risk. You can use `evaluate_solvent_health` to quantify this impact.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/amine-treating-unit-design](https://vinkius.com/en/ai-agent-connect/amine-treating-unit-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amine Treating Unit Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `amine-treating-unit-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amine Treating Unit Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amine-treating-unit-design": {
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
