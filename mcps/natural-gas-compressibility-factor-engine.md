# Natural Gas Compressibility Factor Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/natural-gas-compressibility-factor-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

High-precision Z-factor calculations using industry-standard correlations.

## Description
This MCP server provides high-precision engineering tools for determining the gas compressibility factor (Z-factor). It connects AI agents to advanced thermodynamic correlations like Dranchuk-Abou-Kassem and Standing-Katz. Users can calculate Z-factors using detailed molar compositions or specific gravity, evaluate the impact of sour gases, and validate operating conditions for gas phase stability. It is designed for natural gas engineers and researchers needing accurate pseudo-reduced property derivations.


## Available Tools (4)
- **validate_gas_conditions**: Checks if the provided pressure and temperature are within the valid range for standard compressibility correlations
- **calculate_z_factor_by_composition**: g., '{"methane": 0.9, "ethane": 0.1}').

Calculates the Z-factor using a detailed molar composition of the gas
- **calculate_z_factor_by_gravity**: Calculates the Z-factor when only the specific gravity of the gas is known
- **get_sour_gas_impact**: Evaluates how much the acid gas content is shifting the pseudo-critical properties


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Natural Gas Compressibility Factor Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Z-factor for a gas with 90% methane and 10% ethane at 2000 psia and 150 F."

**🤖 AI Agent:**
> The calculated Z-factor is 0.842, with a pseudo-reduced pressure of 1.45 and pseudo-reduced temperature of 1.62.

---

**👤 You:**
> "What is the impact of 5% H2S on the gas properties?"

**🤖 AI Agent:**
> The acid gas fraction is 0.05, resulting in a critical property shift factor of 1.032.

---

**👤 You:**
> "Calculate Z-factor for a gas with specific gravity 0.65 at 3000 psia and 100 F."

**🤖 AI Agent:**
> The Z-factor is 0.785 based on the Standing-Katz correlation.


## ❓ FAQ

**Q: What correlations are used for Z-factor calculation?**
The engine utilizes the Dranchuk-Abou-Kassem correlation for high-precision composition-based calculations and the Standing-Katz correlation for specific gravity-based calculations.

**Q: How does the engine handle sour gas?**
You can use `get_sour_gas_impact` to evaluate how acid gases like H2S or CO2 shift pseudo-critical properties, ensuring accurate Z-factor results.

**Q: Can I validate if my gas is in a supercritical state?**
Yes, the `validate_gas_conditions` tool checks if the provided pressure and temperature are within valid ranges for standard correlations and identifies supercritical or liquid states.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/natural-gas-compressibility-factor-engine](https://vinkius.com/en/ai-agent-connect/natural-gas-compressibility-factor-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Natural Gas Compressibility Factor Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `natural-gas-compressibility-factor-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Natural Gas Compressibility Factor Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "natural-gas-compressibility-factor-engine": {
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
