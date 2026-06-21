# Global Effective Tax Rate & Pillar Two Compliance MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/global-effective-tax-rate-pillar-two-compliance)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/global-effective-tax-rate-pillar-two-compliance-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/global-effective-tax-rate-pillar-two-compliance-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate global effective tax rates and OECD Pillar Two top-up tax liabilities.

## Description
This MCP server provides a specialized engine for multinational enterprises to ensure compliance with the OECD Pillar Two framework. By using tools like `calculate_jurisdictional_deficiency`, companies can identify jurisdictions where the local effective tax rate falls below the 15% global minimum threshold. The server also enables calculating the weighted average global ETR via `calculate_global_etr` and determining the total enterprise-wide tax obligation, including all top-up taxes, through `calculate_consolidated_burden`. It acts as a critical bridge for AI agents to perform complex international tax computations accurately.


## Available Tools
- **calculate_consolidated_burden**: Provide the final total tax obligation for the entire enterprise including top-up adjustments
- **calculate_global_etr**: Find the single weighted average tax rate for a company's entire global operations
- **calculate_jurisdictional_deficiency**: Determine if a specific country's tax rate is insufficient and calculate the resulting liability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Global Effective Tax Rate & Pillar Two Compliance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if Ireland's 12.5% tax rate requires a top-up tax for a profit of $1,000,000."

**🤖 AI Agent:**
> Yes, Ireland's rate is below the 15% threshold. The top-up tax due is $25,000.

---

**👤 You:**
> "Calculate the global ETR for jurisdictions with profits of $500k at 10% and $500k at 20%."

**🤖 AI Agent:**
> The global effective tax rate for these operations is 15.0%.

---

**👤 You:**
> "What is my total consolidated tax burden if I have $10,000 in local tax and $5,000 in top-up tax?"

**🤖 AI Agent:**
> Your total effective liability is $15,000.


## Installation & Usage

To install and use the **Global Effective Tax Rate & Pillar Two Compliance** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/global-effective-tax-rate-pillar-two-compliance](https://vinkius.com/mcp/global-effective-tax-rate-pillar-two-compliance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
