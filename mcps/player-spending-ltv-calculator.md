# Player Spending LTV Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/player-spending-ltv-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/player-spending-ltv-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/player-spending-ltv-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [gaming](../categories/gaming.md)

Calculate player Lifetime Value (LTV), Breakeven CAC, and retention impact.

## Description
An analytical engine for mobile gaming economics. Use `get_segment_economics` to find the maximum allowable acquisition cost, `get_revenue_distribution` to see segment revenue splits based on the 80/20 rule, and `get_retention_impact` to quantify the financial benefit of reducing churn.


## Available Tools
- **get_retention_impact**: 01 reduction in churn.

Calculate the value of improving player retention by 1%
- **get_revenue_distribution**: Get the theoretical revenue distribution across segments
- **get_segment_economics**: Calculate LTV and Breakeven CAC for a player segment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Player Spending LTV Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the LTV for a whale segment with 5.00 ARPU, 0.02 churn rate, and 70% margin."

**🤖 AI Agent:**
> The calculated LTV for the whale segment is 175.00, with a Breakeven CAC of 175.00.

---

**👤 You:**
> "What is the revenue distribution across segments?"

**🤖 AI Agent:**
> { "free": 0.1, "dolphin": 0.2, "whale": 0.7 }

---

**👤 You:**
> "How much is a 1% reduction in churn worth for a dolphin player with 1.00 ARPU, 0.10 churn, and 70% margin?"

**🤖 AI Agent:**
> Reducing the churn rate by one percentage point results in a value increase of 0.70 per player.


## Installation & Usage

To install and use the **Player Spending LTV Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/player-spending-ltv-calculator](https://vinkius.com/mcp/player-spending-ltv-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
