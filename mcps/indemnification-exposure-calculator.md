# Indemnification Exposure Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/indemnification-exposure-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/indemnification-exposure-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/indemnification-exposure-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate maximum financial exposure in indemnity clauses by assessing contractual caps, carve-outs, and jurisdiction.

## Description
This MCP server provides tools to quantify the potential financial risks associated with indemnification clauses in legal contracts. By analyzing the interaction between contractual caps, specific carve-outs (such as IP infringement or fraud), and jurisdictional legal standards, agents can determine the worst-case exposure scenario. Use `calculate_standard_cap` to find the primary liability ceiling, `evaluate_carveout_impact` to estimate additional risk from exceptions, and `calculate_worst_case_exposure` for a comprehensive breakdown of total potential loss.


## Available Tools
- **evaluate_carveout_impact**: Estimates the additional liability exposure introduced by specific carve-out events
- **calculate_standard_cap**: Calculates the maximum dollar amount allowed under the standard cap
- **calculate_worst_case_exposure**: Aggregates standard caps, carve-outs, and damage type considerations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Indemnification Exposure Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the standard cap for a $500,000 contract with a 2x multiplier."

**🤖 AI Agent:**
> The calculated standard cap is $1,000,000.

---

**👤 You:**
> "What is the worst-case exposure for a $1M contract with a 1x cap and active IP_INFRINGEMENT carve-out?"

**🤖 AI Agent:**
> The total worst-case exposure is $2,000,000 ($1,000,000 standard cap + $1,000,000 from the carve-out).

---

**👤 You:**
> "Estimate the impact of fraud and gross negligence on a $250,000 contract."

**🤖 AI Agent:**
> The additional exposure from these two carve-outs is estimated at $500,000.


## Installation & Usage

To install and use the **Indemnification Exposure Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/indemnification-exposure-calculator](https://vinkius.com/mcp/indemnification-exposure-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
