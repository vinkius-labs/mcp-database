# US Wind Load Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-wind-load-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate wind pressure (psf) based on ASCE 7 standards using regional wind speeds and terrain exposure.

## Description
This MCP server provides structural engineering tools to estimate wind velocity pressure at specific building heights. By utilizing the `lookup_wind_speed` tool, you can retrieve base wind speeds for any US state or county. The `calculate_pressure_at_height` tool then computes the pressure in pounds per square foot (psF) by accounting for terrain roughness (Exposure Categories B, C, or D). For a comprehensive analysis, use `compare_exposure_scenarios` to see how different environmental terrains impact wind force at a single elevation.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Wind Load Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the base wind speed in Miami-Dade, FL?"

**🤖 AI Agent:**
> The base wind speed for Miami-Dade, FL is 150 mph.

---

**👤 You:**
> "Calculate the wind pressure at 30 feet in an open terrain (Category C) with a wind speed of 100 mph."

**🤖 AI Agent:**
> The estimated wind pressure at 30 feet for Category C exposure is approximately 25.1 psf.

---

**👤 You:**
> "Compare the wind pressure at 50 feet for different terrains using a 120 mph wind speed."

**🤖 AI Agent:**
> At 50 feet with 120 mph wind: Category B is approximately 48.5 psf, Category C is approximately 36.2 psf, and Category D is approximately 34.8 psf.


## ❓ FAQ

**Q: What is the purpose of this tool?**
It calculates wind pressure on structures using simplified ASCE 7 methodology, considering regional wind speeds and terrain exposure. Tools available: `your_tool_name`.

**Q: How do I find the wind speed for my location?**
Use the `lookup_wind_speed` tool by providing your US state abbreviation and, optionally, your county name.

**Q: What are exposure categories B, C, and D?**
Category B is for urban/suburban areas; Category C is for open terrain like grasslands; Category D is for smooth surfaces like waterfronts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-wind-load-calculator](https://vinkius.com/mcp/us-wind-load-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Wind Load Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-wind-load-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Wind Load Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-wind-load-calculator": {
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
