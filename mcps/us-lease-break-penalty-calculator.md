# US Lease Break Penalty Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-lease-break-penalty-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/us-lease-break-penalty-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/us-lease-break-penalty-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Estimate financial liabilities and settlement ranges for US residential and commercial lease terminations.

## Description
This MCP server provides specialized tools to calculate the financial impact of breaking a lease in the United States. Using `calculate_gross_loss`, you can determine total unpaid rent. With `get_state_mitigation_duty`, agents can retrieve state-specific legal obligations regarding a landlord's duty to mitigate damages. Finally, `estimate_lease_break_settlement` provides a calculated range for a reasonable settlement, accounting for re-letting costs and mitigation factors.


## Available Tools
- **calculate_gross_loss**: Calculate total uncollected rent
- **get_state_mitigation_duty**: Retrieve state-specific legal mitigation obligations
- **estimate_lease_break_settlement**: Estimate the reasonable settlement range for a lease break


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Lease Break Penalty Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the gross loss for a lease with $2000 monthly rent and 6 months remaining."

**🤖 AI Agent:**
> The total uncollected rent (gross loss) is $12,000.

---

**👤 You:**
> "What are the mitigation duties in California?"

**🤖 AI Agent:**
> In California, there is a very high duty to mitigate damages, focusing on consumer protection.

---

**👤 You:**
> "Estimate a settlement for a commercial lease in Texas with $5000 rent and 12 months left."

**🤖 AI Agent:**
> The estimated settlement range accounts for the gross loss of $60,000 plus re-letting costs, adjusted by Texas's moderate mitigation duty.


## Installation & Usage

To install and use the **US Lease Break Penalty Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-lease-break-penalty-calculator](https://vinkius.com/mcp/us-lease-break-penalty-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
