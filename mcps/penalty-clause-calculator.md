# Penalty Clause Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/penalty-clause-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/penalty-clause-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/penalty-clause-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate contractual penalties, legal ceilings, and estimated judicial reductions based on jurisdiction.

## Description
The Penalty Clause Calculator is a specialized tool for determining the financial impact of contract breaches. It calculates the raw penalty amount using contract value, penalty rate, and delay days via `calculate_raw_penalty`. It also identifies legal maximums for specific jurisdictions like the USA or EU member states using `get_jurisdiction_ceiling`. Finally, it determines the legally recoverable amount after applying jurisdictional caps and estimating potential judicial reductions with `calculate_enforceable_penalty`.


## Available Tools
- **calculate_enforceable_penalty**: Determines the final penalty amount after applying legal caps
- **get_jurisdiction_ceiling**: g., USA, DE, FR).

Retrieves the maximum allowable penalty percentage for a jurisdiction
- **calculate_raw_penalty**: Calculates the initial penalty amount based on contract terms


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Penalty Clause Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the raw penalty for a $10,000 contract with a 5% rate and 15 days of delay."

**🤖 AI Agent:**
> $250.00

---

**👤 You:**
> "What is the legal penalty ceiling for Germany?"

**🤖 AI Agent:**
> 5.00%

---

**👤 You:**
> "If my raw penalty is $1,000 on a $10,000 contract in the USA, what is the enforceable amount?"

**🤖 AI Agent:**
> The applicable penalty is $1,000.00, with a legal ceiling of $1,000.00 and an estimated reduction of $0.00.


## Installation & Usage

To install and use the **Penalty Clause Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/penalty-clause-calculator](https://vinkius.com/mcp/penalty-clause-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
