# Corrosion Kinetics Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/corrosion-kinetics-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculates corrosion current, material loss rates, and analyzes Evans diagrams from electrochemical data.

## Description
This MCP server provides specialized tools for electrochemical analysis. It connects AI agents to kinetic calculations using the Stern-Geary equation. Use `calculate_corrosion_current` to determine instantaneous current density from Tafel slopes and polarization resistance. Use `calculate_corrosion_rate` to convert electrical current into physical material loss. The engine also includes `analyze_evans_diagram` to evaluate kinetic feasibility and `get_polarization_resistance_metrics` for temperature-normalized resistance values. It is compatible with Cursor, VS Code, Claude Desktop, and Windsurf.


## Available Tools (4)
- **analyze_evans_diagram**: Evaluates the relationship between anodic and cathodic branches to check for kinetic feasibility
- **calculate_corrosion_current**: Determines the instantaneous corrosion current density based on Tafel extrapolation
- **calculate_corrosion_rate**: Converts electrical current density into a physical material loss rate
- **get_polarization_resistance_metrics**: Validates and retrieves resistance metrics used for further kinetic calculations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Corrosion Kinetics Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the corrosion current density if the anodic Tafel slope is 0.12, cathodic Tafel slope is 0.15, and polarization resistance is 500 ohms."

**🤖 AI Agent:**
> The corrosion current density is 0.00148 A/cm².

---

**👤 You:**
> "What is the corrosion rate for a current density of 0.002 A/cm², a material density of 7.87 g/cm³, and an equivalent weight of 27.92?"

**🤖 AI Agent:**
> The corrosion rate is 0.00057 g/cm² per unit time.

---

**👤 You:**
> "Check the equilibrium of an Evans diagram with anodic current 1.2, cathodic current 1.2, and corrosion potential 0.5."

**🤖 AI Agent:**
> The system is in equilibrium.


## ❓ FAQ

**Q: What data is required for corrosion current calculation?**
To use `calculate_corrosion_current`, you must provide the anodic Tafel slope, the cathodic Tafel slope, and the measured polarization resistance.

**Q: How is the corrosion rate determined?**
The `calculate_corrosion_rate` tool converts current density into physical mass loss by using the material density and the electrochemical equivalent weight.

**Q: Can I analyze Evans diagrams directly?**
Yes, the `analyze_evans_diagram` tool evaluates the relationship between anodic and cathodic branches to check for kinetic equilibrium.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/corrosion-kinetics-engine](https://vinkius.com/ai-agent-connect/corrosion-kinetics-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Corrosion Kinetics Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `corrosion-kinetics-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Corrosion Kinetics Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "corrosion-kinetics-engine": {
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
