# Water Heater Comparator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/water-heater-comparator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/water-heater-comparator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/water-heater-comparator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Compare the operational costs and carbon footprint of electric, gas, and solar thermal water heating systems.

## Description
This MCP server provides analytical tools to quantify the financial and environmental impact of different water heating technologies. Use `evaluate_electric_system` to calculate costs and CO2 emissions for electric showers, `evaluate_gas_system` to determine the footprint of gas-powered heaters, or `evaluate_solar_thermal_system` to estimate the efficiency and backup energy needs of solar thermal setups based on your specific usage profile.


## Available Tools
- **evaluate_electric_system**: Calculate cost and emissions for an electric shower setup
- **evaluate_gas_system**: Calculate cost and emissions for a gas-powered water heater
- **evaluate_solar_thermal_system**: Calculate cost and emissions for a solar thermal system


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Water Heater Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the cost and emissions for a 10-minute shower for 4 people at 40°C using an electric system."

**🤖 AI Agent:**
> The `evaluate_electric_system` tool will return the total cost, CO2 emissions in kg, and the volume of water used for this profile.

---

**👤 You:**
> "What is the environmental impact of a gas heater for 2 people showering for 15 minutes at 38°C?"

**🤖 AI Agent:**
> By using `evaluate_gas_system`, you can see the specific carbon footprint and operational cost associated with natural gas consumption for this usage.

---

**👤 You:**
> "Compare solar thermal efficiency for a large family."

**🤖 AI Agent:**
> The `evaluate_solar_thermal_system` tool will provide the percentage of heat provided by solar energy and the required backup heating costs.


## Installation & Usage

To install and use the **Water Heater Comparator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/water-heater-comparator](https://vinkius.com/mcp/water-heater-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
