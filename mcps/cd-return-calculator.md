# CD Return Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cd-return-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cd-return-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cd-return-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate potential returns on Certificates of Deposit (CD) and compare them against market benchmarks like HYSA and Money Market funds.

## Description
The CD Return Calculator is a specialized financial tool designed to help you project the growth of your investments in Certificates of Deposit. By providing the principal amount, APY, and term duration, you can use tools like `calculate_cd_yield` to see exactly how much interest you will earn and what your final balance will be. The server also provides context by using `fetch_market_benchmarks` to compare your CD's performance against current High-Yield Savings Account (HYSA) and Money Market rates. Finally, the `generate_investment_comparison` tool produces a clear assessment of whether your CD is outperforming liquid market alternatives.


## Available Tools
- **calculate_cd_yield**: Calculates the growth of an investment based on CD terms and compounding interest
- **fetch_market_benchmarks**: Retrieves the current hardcoded benchmark rates for liquid alternatives based on a given interest rate level
- **generate_investment_comparison**: Produces a high-level comparison between the CD investment and market alternatives


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CD Return Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the return for a $5,000 CD with 4.5% APY for 12 months, compounding monthly."

**🤖 AI Agent:**
> For a $5,000 deposit at 4.5% APY over 12 months with monthly compounding, your total interest earned will be $229.36, resulting in a final balance of $5,229.36.

---

**👤 You:**
> "Is a 4% CD better than current market benchmarks?"

**🤖 AI Agent:**
> Based on current benchmarks, a 4% CD is performing similarly to the available HYSA and Money Market rates in this tier.

---

**👤 You:**
> "Compare a $10,000 CD at 5% APY for 24 months against HYSA rates."

**🤖 AI Agent:**
> A $10,000 CD at 5% APY for 24 months will yield a final balance of $11,049.41. This outperforms the current HYSA benchmark rate.


## Installation & Usage

To install and use the **CD Return Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cd-return-calculator](https://vinkius.com/mcp/cd-return-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
