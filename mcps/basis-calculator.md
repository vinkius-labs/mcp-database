# Basis Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/basis-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/basis-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/basis-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate and analyze commodity basis by comparing local physical prices against exchange futures.

## Description
The Basis Calculator MCP server provides AI agents with specialized tools to determine market parity for commodities. Using `calculate_current_basis`, agents can compute the absolute basis value and identify if a market is Above or Below Parity. The server also includes `get_historical_averages` to benchmark current prices against historical regional data, and `get_seasonality_trend` to predict basis movements during Harvest or Off-season periods.


## Available Tools
- **calculate_current_basis**: Positive is Above Parity, negative is Below Parity.

Determine the absolute basis value and its market classification based on current pricing
- **get_historical_averages**: Retrieve hardcoded historical basis averages for specific regions and commodities
- **get_seasonality_trend**: Identify the expected basis movement pattern for a specific period in the agricultural cycle


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Basis Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the basis if the physical price is 120 and the future price is 115."

**🤖 AI Agent:**
> The absolute basis value is 5, which indicates a market position of Above Parity.

---

**👤 You:**
> "What is the historical average basis for Mato Grosso - Soy?"

**🤖 AI Agent:**
> The historical average basis for Mato Grosso - Soy is retrieved from the registry to provide context.

---

**👤 You:**
> "What is the expected trend during the Harvest season?"

**🤖 AI Agent:**
> During the Harvest season, the basis movement direction is typically identified as part of the seasonal behavior profile.


## Installation & Usage

To install and use the **Basis Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/basis-calculator](https://vinkius.com/mcp/basis-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
