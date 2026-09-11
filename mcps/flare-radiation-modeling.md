# Flare Radiation Modeling MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/flare-radiation-modeling)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate thermal radiation intensity, exclusion zones, and stack heights using API 521 standards.

## Description
This MCP server provides technical simulation tools for flare systems based on the API 521 standard. It allows AI agents to model thermal radiation intensity, identify safety exclusion zones for personnel and equipment, and determine the minimum required stack height. The tools account for flare type, gas composition, mass flow rates, wind-induced flame tilt, and solar radiation to ensure accurate safety modeling.


## Available Tools (4)
- **calculate_radiation_intensity**: Determines the thermal radiation flux at a specific coordinate relative to the flare
- **calculate_required_stack_height**: Determines the minimum height the flare stack must be to meet safety standards
- **determine_exclusion_zones**: Identifies the safety radii required to protect personnel and equipment
- **get_gas_energy_content**: Retrieves the specific energy (heating value) for a given gas mixture


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flare Radiation Modeling** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the radiation intensity at 50 meters for an elevated flare with a methane-heavy gas composition and a flow rate of 10 kg/s?"

**🤖 AI Agent:**
> The calculated radiation intensity at 50 meters is 4.2 kW/m².

---

**👤 You:**
> "Calculate the required stack height for an elevated flare to keep ground radiation below 1.5 kW/m² given a 10 kg/s flow rate and 5 m/s wind."

**🤖 AI Agent:**
> The minimum required stack height is 24.5 meters.

---

**👤 You:**
> "What is the personnel exclusion zone for a ground flare with a flow rate of 5 kg/s and a wind speed of 10 m/s?"

**🤖 AI Agent:**
> The personnel exclusion radius is 32.0 meters.


## ❓ FAQ

**Q: How does this server handle wind effects?**
The `determine_exclusion_zones` and `calculate_required_stack_height` tools incorporate wind speed to model flame tilt, which shifts the radiation profile and affects safety distances.

**Q: Can I calculate radiation for specific gas mixtures?**
Yes, you can use `calculate_radiation_intensity` by providing a JSON string of the gas composition to determine the heat release rate and resulting flux.

**Q: What standards does this model follow?**
The modeling logic is built upon the API 521 standard for flare systems.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/flare-radiation-modeling](https://vinkius.com/en/ai-agent-connect/flare-radiation-modeling)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flare Radiation Modeling** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flare-radiation-modeling` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flare Radiation Modeling** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flare-radiation-modeling": {
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
