# ARR Bridge Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arr-bridge-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/arr-bridge-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/arr-bridge-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Quantify and visualize Annual Recurring Revenue (ARR) movements by detailing the specific drivers of revenue expansion and contraction over time.

## Description
The ARR Bridge Calculator is a specialized financial engine designed to decompose Annual Recurring Revenue (ARR) changes into their fundamental drivers. By analyzing components such as `get_monthly_bridge_summary` for specific months, `get_bridge_waterfall_sequence` for chronological revenue flows, and `analyze_component_trends` for growth or decline patterns, users can gain deep insights into their subscription business health. This tool provides a clear view of New ARR, Expansion, Reactivation, Contraction, and Churned ARR, allowing for precise tracking of Net New ARR and long-term revenue trends.


## Available Tools
- **analyze_component_trends**: Analyzes how specific revenue drivers are growing or shrinking over a period
- **get_bridge_waterfall_sequence**: Generates a chronological sequence of monthly bridge summaries over a specified range
- **get_monthly_bridge_summary**: Provides a detailed breakdown of all ARR movement components for a single, specific month


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ARR Bridge Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the ARR breakdown for January 2024."

**🤖 AI Agent:**
> In January 2024, your New ARR was $50,000, Expansion was $10,000, Reactivation was $5,000, while Contraction was $2,000 and Churn was $3,000, resulting in a Net New ARR of $60,000.

---

**👤 You:**
> "What is the revenue trend for expansion from 2024-01 to 2024-06?"

**🤖 AI Agent:**
> The expansion component shows an improving trend, with a value of $15,000 in June 2024, representing a 12% increase compared to the previous period.

---

**👤 You:**
> "Give me a waterfall sequence of my revenue from 2024-01 to 2024-03."

**🤖 AI Agent:**
> The sequence shows: Jan 2024 ($60,000 Net New), Feb 2024 ($55,000 Net New), and Mar 2024 ($62,000 Net New).


## Installation & Usage

To install and use the **ARR Bridge Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arr-bridge-calculator](https://vinkius.com/mcp/arr-bridge-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
