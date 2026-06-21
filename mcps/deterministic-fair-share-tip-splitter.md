# Deterministic Fair-Share Tip Splitter MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deterministic-fair-share-tip-splitter)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/deterministic-fair-share-tip-splitter-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/deterministic-fair-share-tip-splitter-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transform your AI into a hyper-precise ledger. Mathematically split complex restaurant bills, proportionally distribute taxes and tips, and resolve fractional penny discrepancies instantly.

## Description
Splitting a restaurant bill with shared appetizers, individual drinks, and group tips is a mathematical nightmare for LLMs. They frequently hallucinate decimal distributions and fail to balance the final grand total. The Tip Splitter MCP offloads this exact calculation to a rigorous V8 mathematical engine.

### The Superpowers
- **Proportional Taxation & Tipping:** The engine automatically calculates each person's base subtotal based on the specific items they consumed (or shared), and then proportionally applies the exact tax and tip burden to each individual.
- **Penny Reconciliation Algorithm:** When fractional cents create a discrepancy between the calculated individual totals and the actual receipt grand total, the engine automatically reconciles the missing or extra penny to guarantee 100% mathematical closure.
- **Shared Consumption Mapping:** Allows mapping a single item (like 'Nachos') to multiple consumers (e.g., 'Alice' and 'Bob'). The engine dynamically splits the price before applying secondary rates.
- **Zero-Dependency Execution:** Operates entirely natively within the V8 runtime, guaranteeing extreme speed and precision without pulling heavy external libraries.


## Available Tools
- **split_bill**: You must provide the items as a stringified JSON array, along with the total taxAmount and tipPercentage.

Deterministically calculates individual bill shares, proportionally distributing taxes and tips among consumers based on their exact items, and resolving rounding discrepancies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deterministic Fair-Share Tip Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Split this bill: Burger ($15) for Alice, Salad ($12) for Bob, and shared Nachos ($10) for both. Tax is $3.50 and tip is 20%."

**🤖 AI Agent:**
> Using the split_bill tool: The grand total is $47.90. Alice owes $25.89 (base: $20.00) and Bob owes $22.01 (base: $17.00).

---

**👤 You:**
> "Three of us had a $90 steak dinner (all shared). Tax $8, tip 15%. How much each?"

**🤖 AI Agent:**
> Using the split_bill tool: The grand total is $111.50. Thanks to the Penny Reconciliation Algorithm, Person 1 pays $37.16, while Person 2 and Person 3 pay $37.17 each to exactly cover the bill.

---

**👤 You:**
> "Calculate the fair split for a $45 bill where John had a $30 wine and Sarah had a $15 pasta. Tax $4, tip 18%."

**🤖 AI Agent:**
> Using the split_bill tool: Since John's base item was 66.6% of the bill, he correctly absorbs 66.6% of the tax and tip burden. John owes $38.07, and Sarah owes $19.03. Grand total: $57.10.


## Installation & Usage

To install and use the **Deterministic Fair-Share Tip Splitter** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deterministic-fair-share-tip-splitter](https://vinkius.com/mcp/deterministic-fair-share-tip-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
