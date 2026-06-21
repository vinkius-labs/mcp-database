# Lime Requirement Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lime-requirement-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lime-requirement-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lime-requirement-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate precise limestone dosage and total application costs using base saturation and SMP buffer methods.

## Description
This MCP server provides specialized agricultural tools to determine the exact amount of lime needed for soil correction. Use `calculate_base_saturation_dosage` to calculate requirements based on current and target base saturation (V%), soil CTC, and lime PRNT. You can also use `calculate_smp_dosage` to assess needs via the SMP buffer method, and `calculate_total_expenditure` to project total mass needed and financial investment for a specific field area.


## Available Tools
- **calculate_base_saturation_dosage**: Calculates the amount of lime required to reach a desired base saturation level
- **calculate_smp_dosage**: Determines the lime requirement based on the SMP buffer capacity measurements
- **calculate_total_expenditure**: Estimates the total financial investment required for a specific field area


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lime Requirement Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate lime dosage for a soil with 40% V%, target 65%, CTC of 10, and PRNT of 85%."

**🤖 AI Agent:**
> The `calculate_base_saturation_dosage` tool would calculate the required dosage based on these parameters.

---

**👤 You:**
> "What is the cost for 50 hectares if I need 2 tonnes per hectare at $150 per tonne?"

**🤖 AI Agent:**
> Using `calculate_total_expenditure`, the total mass needed is 100 tonnes, with a total cost of $15,000.

---

**👤 You:**
> "Determine lime needs using SMP value of 4.5 and target of 6.0."

**🤖 AI Agent:**
> The `calculate_smp_dosage` tool will compute the necessary dosage per hectare to reach the target equilibrium.


## Installation & Usage

To install and use the **Lime Requirement Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lime-requirement-calculator](https://vinkius.com/mcp/lime-requirement-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
