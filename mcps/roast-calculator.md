# Roast Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/roast-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/roast-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/roast-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [culinary](../categories/culinary.md)

Precise cooking time, resting duration, and carryover temperature predictions for meat roasting.

## Description
The Roast Calculator MCP server provides specialized culinary computations for professional and home roasting. By connecting AI agents to precise thermal models, it enables accurate predictions of cooking duration using `calculate_cooking_duration`, recommended resting periods via `calculate_rest_duration`, and temperature shifts during the rest phase with `estimate_carrylag_impact`.


## Available Tools
- **estimate_carryover_impact**: Estimate the temperature increase due to carryover cooking
- **calculate_cooking_duration**: Calculate the estimated total cooking time for a roast
- **calculate_rest_duration**: Calculate the recommended resting time for a roast


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Roast Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long will a 2kg Beef roast take at 150C?"

**🤖 AI Agent:**
> You should use the `calculate_cooking_duration` tool with meatType: 'Beef', weightKg: 2, and ovenTemperatureCelsius: 150 to get the exact estimate.

---

**👤 You:**
> "How much will the temperature rise for a Pork roast?"

**🤖 AI Agent:**
> To find this, use `estimate_carryover_impact` with your removal and target temperatures.

---

**👤 You:**
> "What is the resting time for a 5kg roast?"

**🤖 AI Agent:**
> Use `calculate_rest_duration` with weightKg: 5 to determine the optimal rest period.


## Installation & Usage

To install and use the **Roast Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/roast-calculator](https://vinkius.com/mcp/roast-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
