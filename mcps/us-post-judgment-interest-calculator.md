# US Post-Judgment Interest Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-post-judgment-interest-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/us-post-judgment-interest-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/us-post-judgment-interest-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate US Federal post-judgment interest accrual based on 28 U.S.C. § 1961 and Treasury Bill rates.

## Description
This MCP server provides precise calculations for US Federal post-judgment interest as mandated by 28 U.S.C. § 1961. By using weekly Treasury Bill rates, the server allows AI agents to determine exactly how much interest has accumulated on a court judgment between a specific judgment date and a target payment date. Use `rate_lookup` to find the annual rate for any given week, `interest_accrual_calc` to compute total interest and updated balance, or `interest_scenario_comparison` to evaluate the cost difference between early and late payments.


## Available Tools
- **interest_accrual_calc**: Calculate total interest and balance for a judgment
- **rate_lookup**: Look up the annual interest rate for a specific date
- **interest_scenario_comparison**: Compare interest costs between two payment dates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Post-Judgment Interest Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much interest has accrued on a $10,000 judgment from 2024-01-01 to 2024-06-01?"

**🤖 AI Agent:**
> The total interest accrued on the $10,000 judgment from January 1, 2024, to June 1, 2024, is $150.00, bringing the total balance to $10,150.00.

---

**👤 You:**
> "What was the Treasury Bill rate for 2024-02-15?"

**🤖 AI Agent:**
> The annual interest rate applicable for the week containing February 15, 2024, was 5.35%.

---

**👤 You:**
> "Compare interest costs for a $5,000 judgment if I pay on 2024-12-01 versus 2025-03-01."

**🤖 AI Agent:**
> Choosing to pay on March 1, 2025, instead of December 1, 2024, will result in an additional interest cost of $42.50.


## Installation & Usage

To install and use the **US Post-Judgment Interest Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-post-judgment-interest-calculator](https://vinkius.com/mcp/us-post-judgment-interest-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
