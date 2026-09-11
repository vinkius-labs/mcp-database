# Reserves Estimation Volumetric MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/reserves-estimation-volumetric)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate oil and gas in place and recoverable reserves using the volumetric method.

## Description
This MCP server provides specialized tools for petroleum engineering calculations. It allows AI agents to estimate Original Oil/Gas in Place (OOIP/OGIP) using `calculate_oil_in_place`, determine extractable volumes with `calculate_recoverable_reserves`, and classify reserves into Proved, Probable, and Possible categories via `estimate_reserve_categories`. It also includes `validate_reservoir_parameters` to ensure physical consistency of reservoir inputs.


## Available Tools (4)
- **validate_reservoir_parameters**: Checks the physical consistency of a set of reservoir inputs
- **calculate_oil_in_place**: Calculates the total original oil in place (OOIP) based on reservoir physical properties
- **calculate_recoverable_reserves**: Calculates the volume of oil that can be extracted
- **estimate_reserve_categories**: Applies uncertainty ranges to the recoverable reserves to provide P1, P2, and P3 classifications


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reserves Estimation Volumetric** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the oil in place for a reservoir with 500 area, 50 thickness, 0.2 porosity, 0.3 water saturation, and 1.2 formation volume factor."

**🤖 AI Agent:**
> The total original oil in place is 42,000 units.

---

**👤 You:**
> "If I have 100,000 units of oil in place and a recovery factor of 0.3, what are the recoverable reserves?"

**🤖 AI Agent:**
> The recoverable reserves are 30,000 units.

---

**👤 You:**
> "Estimate the P1, P2, and P3 reserves for 50,000 recoverable reserves using confidence multipliers of 0.9, 0.7, and 0.5."

**🤖 AI Agent:**
> The reserve categories are: Proved (P1) is 45,000, Probable (P2) is 35,000, and Possible (P3) is 25,000.


## ❓ FAQ

**Q: What is the volumetric method?**
The volumetric method is a technique used to estimate the total volume of hydrocarbons in a reservoir based on its physical properties like area, thickness, porosity, and saturation.

**Q: How are reserve categories defined?**
Reserves are categorized into Proved (P1), Probable (P2), and Possible (P3) based on the level of geological and engineering confidence applied to the recoverable volumes.

**Q: Can I validate my reservoir data before calculating reserves?**
Yes, you can use the `validate_reservoir_parameters` tool to check if your area, thickness, porosity, and water saturation values are physically consistent and within valid ranges.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/reserves-estimation-volumetric](https://vinkius.com/ai-agent-connect/reserves-estimation-volumetric)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reserves Estimation Volumetric** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reserves-estimation-volumetric` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reserves Estimation Volumetric** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reserves-estimation-volumetric": {
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
