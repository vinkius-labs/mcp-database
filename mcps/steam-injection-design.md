# Steam Injection Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/steam-injection-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design steam injection processes for heavy oil recovery, calculating injection rates, steam quality, and expected oil recovery.

## Description
This MCP server provides specialized tools for designing thermal enhanced oil recovery (EOR) processes. It allows AI agents to calculate optimal steam injection rates using `get_injection_rate`, determine steam quality with `calculate_steam_properties`, define well pattern geometry via `design_pattern_geometry`, and predict total oil recovery using `estimate_oil_recovery`. The design accounts for critical reservoir factors like viscosity, depth, thickness, and gravity override to ensure efficient heat delivery and oil movement.


## Available Tools (4)
- **get_injection_rate**: Determines the optimal rate of steam injection based on reservoir properties and steam supply
- **design_pattern_geometry**: Determines the spatial arrangement and size of the well patterns
- **calculate_steam_properties**: Calculates the necessary steam quality and characteristics for the design
- **estimate_oil_recovery**: Predicts the total volume of oil that can be recovered using the designed steam injection parameters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steam Injection Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the optimal steam injection rate for an oil with 500 cP viscosity at 1000m depth, 50m thickness, and 500 units of steam availability?"

**🤖 AI Agent:**
> The optimal steam injection rate is 125.5 units, optimized for the reservoir.

---

**👤 You:**
> "Calculate the steam quality if the injection rate is 150 and steam availability is 200."

**🤖 AI Agent:**
> The calculated steam quality is 0.75 with a thermal efficiency of 0.82.

---

**👤 You:**
> "Estimate the oil recovery for 200 cP oil, 150 injection rate, 500 pattern size, 0.8 steam quality, and 40m thickness."

**🤖 AI Agent:**
> The expected oil recovery is 12,500 barrels with a recovery factor of 0.35.


## ❓ FAQ

**Q: How do I calculate the optimal steam injection rate?**
You can use the `get_injection_rate` tool by providing the oil viscosity, reservoir depth, thickness, and available steam supply.

**Q: Can this tool predict the total oil recovered?**
Yes, the `estimate_oil_recovery` tool predicts the total volume of oil recovered and the recovery factor based on your design parameters.

**Q: Does the design account for gravity override?**
Yes, the `design_pattern_geometry` tool considers reservoir thickness and steam quality to adjust pattern size for gravity override effects.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/steam-injection-design](https://vinkius.com/en/ai-agent-connect/steam-injection-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steam Injection Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `steam-injection-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steam Injection Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steam-injection-design": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
