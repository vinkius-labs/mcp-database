# Change Order Impact Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/change-order-impact-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/change-order-impact-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/change-order-impact-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Quantify the financial and schedule consequences of scope changes in construction projects.

## Description
This MCP server provides essential tools for construction and project managers to manage scope creep. Use `calculate_change_order_prce` to determine the total price impact of a single change by applying overhead and profit margins to direct costs. With `calculate_cumulative_impact`, you can track how multiple changes affect the overall contract value and project timeline. Additionally, use `assess_project_risk_level` to identify if scope drift has pushed your project into high-risk territory based on cumulative change order volume.


## Available Tools
- **assess_project_risk_level**: Categorizes the financial health of the project based on scope drift
- **calculate_change_order_price**: Determines the total price charged to the client for a single specific scope change
- **calculate_cumulative_impact**: Calculates the total financial and schedule impact on a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Change Order Impact Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the price for a change order with $5000 direct cost and 20% markup."

**🤖 AI Agent:**
> The total change order price is $6,000.00, which includes a markup amount of $1,000.00.

---

**👤 You:**
> "What is the cumulative impact if my original contract was $100,000, I have $15,000 in previous changes, and this new change is $5,000 with a 2-day delay?"

**🤖 AI Agent:**
> The updated contract value is $120,000.00. The total change order volume is 20% of the original contract, and the estimated project delay is 2 days.

---

**👤 You:**
> "Assess risk for a $50,000 contract with $10,000 in total change orders."

**🤖 AI Agent:**
> The project is at medium risk level because the percentage drift is 20.00%.


## Installation & Usage

To install and use the **Change Order Impact Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/change-order-impact-calculator](https://vinkius.com/mcp/change-order-impact-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
