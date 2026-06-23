# Lighting Power Density (LPD) Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lighting-power-density-lpd-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sustainability](../categories/sustainability.md)

Calculate LPD, verify ASHRAE 90.1 compliance, and estimate LED energy savings.

## Description
This MCP server provides specialized tools for building energy efficiency analysis. Use `calculate_lpd_value` to determine the wattage per square foot of a space, `verify_ashrae_compliance` to check if your lighting setup meets ASHRAE 90.1 occupancy limits, and `estimate_led_energy_savings` to project annual kWh savings when retrofitting with LED fixtures.


## Available Tools (3)
- **calculate_lpd_value**: Calculate the Lighting Power Density (LPD) for a space
- **estimate_led_energy_savings**: Estimate annual energy savings from an LED retrofit
- **verify_ashrae_compliance**: Verify if the current LPD meets ASHRAE 90.1 standards


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lighting Power Density (LPD) Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the LPD for a 5000 sq ft space with 15000W of lighting?"

**🤖 AI Agent:**
> The calculated Lighting Power Density (LPD) is 3.0 W/SF.

---

**👤 You:**
> "Is an LPD of 1.2 W/SF compliant for an Office space?"

**🤖 AI Agent:**
> Yes, the lighting setup is compliant with ASHRAE 90.1 standards.

---

**👤 You:**
> "How much energy will I save if I switch from 60W bulbs to 15W LEDs in a 2000 sq ft area with 2500 annual operating hours?"

**🤖 AI Agent:**
> The retrofit will result in an annual savings of 150 kWh, representing a 75% reduction in energy consumption.


## ❓ FAQ

**Q: How do I calculate the LPD for my space?**
Use the `calculate_lpd_value` tool by providing the total wattage of all fixtures and the total area in square feet.

**Q: What standards does this tool use for compliance?**
The `verify_ashrae_compliance` tool uses hardcoded limits based on the ASHRAE 90.1 standard for various occupancy types like Office, Retail, and Warehouse.

**Q: Can I estimate how much money I'll save with LEDs?**
Yes, the `estimate_led_energy_savings` tool calculates the projected annual kWh reduction and percentage decrease in power usage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lighting-power-density-lpd-calculator](https://vinkius.com/mcp/lighting-power-density-lpd-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lighting Power Density (LPD) Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lighting-power-density-lpd-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lighting Power Density (LPD) Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lighting-power-density-lpd-calculator": {
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
