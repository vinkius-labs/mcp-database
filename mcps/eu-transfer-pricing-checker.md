# EU Transfer Pricing Checker MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eu-transfer-pricing-checker)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eu-transfer-pricing-checker-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eu-transfer-pricing-checker-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Verify intercompany transaction compliance with OECD Arm's Length Principle using industry benchmarks.

## Description
The EU Transfer Pricing Checker is a specialized compliance engine designed to ensure that intercompany transactions between related entities adhere to the OECD Arm's Length Principle. By comparing applied margins against industry-standard benchmarks, it identifies potential tax adjustment risks. AI agents can use tools like `check_compliance` to verify if a specific margin falls within established ranges, `evaluate_risk_impact` to assess the severity of deviations, and `get_benchmark_ranges` to retrieve market-standard minimum and maximum thresholds for various sectors and functions.


## Available Tools
- **get_benchmark_ranges**: Retrieves the hardcoded market-standard ranges
- **check_compliance**: Checks if a transaction margin falls within the established arm's length range
- **evaluate_risk_impact**: Determines the level of tax audit risk and potential severity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EU Transfer Pricing Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if a 5% margin in the Manufacturing sector for Distribution using TNMM is compliant."

**🤖 AI Agent:**
> The `check_compliance` tool will analyze the 5% margin against the Manufacturing/Distribution benchmark for TNMM and return whether it falls within the arm's length range.

---

**👤 You:**
> "What is the tax risk if my applied margin is 15% in Technology/Services using Cost Plus?"

**🤖 AI Agent:**
> By calling `evaluate_risk_impact`, you can determine the specific risk level (Low, Medium, or High) and the potential severity of a tax adjustment for that 15% margin.

---

**👤 You:**
> "Show me all available benchmark ranges for the Retail sector in Logistics."

**🤖 AI Agent:**
> The `get_benchmark_ranges` tool will return a list of all recognized transfer pricing methods and their corresponding min/max margins for the Retail sector in Logistics.


## Installation & Usage

To install and use the **EU Transfer Pricing Checker** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eu-transfer-pricing-checker](https://vinkius.com/mcp/eu-transfer-pricing-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
