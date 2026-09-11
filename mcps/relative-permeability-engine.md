# Relative Permeability Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/relative-permeability-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Generates multi-phase relative permeability curves using Corey and empirical models.

## Description
This MCP server provides specialized tools for reservoir engineering. It allows AI agents to calculate multi-phase flow behavior using the `get_corey_curves` tool for fundamental two-phase modeling, or `get_three_phase_permeability` for simultaneous oil, water, and gas flow. It also supports `get_hysteresis_adjustment` to account for saturation history and `get_empirical_correlation` for established rock-specific relationships.


## Available Tools (4)
- **get_empirical_correlation**: Provides permeability values based on established empirical relationships
- **get_corey_curves**: Generates fundamental two-phase relative permeability curves based on the Corey model
- **get_hysteresis_adjustment**: Modifies existing permeability curves to account for the direction of saturation change
- **get_three_phase_permeability**: Calculates the simultaneous flow capabilities for oil, water, and gas


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Relative Permeability Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate Corey curves for a water-wet sandstone with 0.2 irreducible water saturation and 0.3 residual oil saturation."

**🤖 AI Agent:**
> The generated curves show water permeability increasing from 0.0 at 0.2 saturation to its maximum, while oil permeability decreases from its maximum at 0.2 saturation towards 0.0 at 0.7 saturation.

---

**👤 You:**
> "What are the permeability values for water, oil, and gas when water saturation is 0.4, oil is 0.5, and gas is 0.1 in a carbonate rock?"

**🤖 AI Agent:**
> For the specified saturations in carbonate rock, the effective permeabilities are krw: 0.15, kro: 0.25, and krg: 0.08.

---

**👤 You:**
> "Apply a hysteresis adjustment for imbibition to a base curve with a trapping coefficient of 0.1."

**🤖 AI Agent:**
> The adjusted curve shows a reduction in non-wetting phase permeability due to the applied trapping coefficient.


## ❓ FAQ

**Q: How do I calculate curves for a water-wet sandstone?**
You can use the `get_corey_curves` tool by specifying 'sandstone' as the rockType and 'water-wet' as the wettability.

**Q: Can I account for gas trapping during imbibition?**
Yes, use the `get_hysteresis_adjustment` tool with the saturationHistory set to 'imbibition' to apply trapping effects.

**Q: Does the engine support three-phase flow calculations?**
Yes, the `get_three_phase_permeability` tool calculates simultaneous flow for oil, water, and gas phases.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/relative-permeability-engine](https://vinkius.com/ai-agent-connect/relative-permeability-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Relative Permeability Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `relative-permeability-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Relative Permeability Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "relative-permeability-engine": {
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
