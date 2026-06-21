# US GAAP & IFRS 15 Revenue Recognition MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-gaap-ifrs-15-revenue-recognition)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/us-gaap-ifrs-15-revenue-recognition-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/us-gaap-ifrs-15-revenue-recognition-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Automate ASC 606 and IFRS 15 revenue recognition by identifying obligations, allocating prices, and calculating progress.

## Description
This MCP server provides a specialized engine for implementing the five-step model of ASC 606 and IFRS 15. It allows AI agents to automate complex financial calculations required for revenue recognition. Use `identify_performance_obligations` to analyze contract items, `allocate_transaction_price` to distribute total consideration based on relative standalone selling prices, and `calculate_revenue_recognition` to determine earned versus deferred revenue based on completion progress.


## Available Tools
- **allocate_transaction_price**: Distribute total transaction price across performance obligations
- **calculate_revenue_recognition**: Calculate recognized and deferred revenue
- **identify_performance_obligations**: Analyze contract items to determine performance obligations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US GAAP & IFRS 15 Revenue Recognition** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a contract with two items: 'Software License' and 'Support Services'. How many performance obligations are there?"

**🤖 AI Agent:**
> The `identify_performance_obligations` tool identifies 2 distinct performance obligations: Software License and Support Services.

---

**👤 You:**
> "Allocate a $10,000 total price between 'License' ($8,000 SSP) and 'Support' ($2,000 SSP)."

**🤖 AI Agent:**
> The allocated amounts are: License: $8,000 and Support: $2,000.

---

**👤 You:**
> "If I have an allocated amount of $5,000 and I am 40% complete, how much revenue is recognized?"

**🤖 AI Agent:**
> $2,000 has been recognized as revenue, and $3,000 remains as deferred revenue.


## Installation & Usage

To install and use the **US GAAP & IFRS 15 Revenue Recognition** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-gaap-ifrs-15-revenue-recognition](https://vinkius.com/mcp/us-gaap-ifrs-15-revenue-recognition)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
