# Transfer Pricing Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/transfer-pricing-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/transfer-pricing-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/transfer-pricing-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Verify arm's length compliance for related-party transactions using CUP, Cost Plus, and Resale Minus methods.

## Description
The Transfer Pricing Calculator ensures that transactions between related parties follow the Arm's Length Principle. By using tools like `get_industry_benchmarks`, `verify_cost_plus_compliance`, `verify_resale_minus_compliance`, and `verify_cup_equivalence`, businesses can determine if their pricing strategies align with industry-standard profit margins and market benchmarks, mitigating tax risks.


## Available Tools
- **get_industry_benchmarks**: Retrieves the acceptable arm's length profit margin bounds for a specific industry sector
- **verify_cup_equivalence**: Evaluates if a transaction price is sufficiently similar to a known market benchmark price
- **verify_resale_minus_compliance**: Determines if the gross margin from a resale transaction is within acceptable industry bounds
- **verify_cost_plus_compliance**: Determines if a transaction's markup on cost is within the allowed arm's length range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Transfer Pricing Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is a 15% markup on a $100 unit cost compliant in the Manufacturing sector?"

**🤖 AI Agent:**
> The applied markup is 15%. Based on the Manufacturing sector benchmarks, this falls within the acceptable arm's length range.

---

**👤 You:**
> "Check if a resale price of $500 with a purchase price of $450 is compliant for Retail."

**🤖 AI Agent:**
> The gross margin is 10%. For the Retail sector, this is within the allowed arm's length bounds.

---

**👤 You:**
> "Compare a transaction price of $95 to a market benchmark of $100 with a 2% tolerance."

**🤖 AI Agent:**
> The price variance is 5%. Since this exceeds the allowed tolerance of 2%, the transaction is not compliant.


## Installation & Usage

To install and use the **Transfer Pricing Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/transfer-pricing-calculator](https://vinkius.com/mcp/transfer-pricing-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
