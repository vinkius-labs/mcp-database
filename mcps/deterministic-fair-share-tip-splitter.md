# Deterministic Fair-Share Tip Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deterministic-fair-share-tip-splitter)
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


## ❓ FAQ

**Q: How does it handle shared items like an appetizer?**
The agent passes an array of 'consumers' for each item. If 'Nachos' ($15) has consumers ['John', 'Jane'], the engine automatically divides the base cost ($7.50 each) before proportionally applying their individual tax and tip burden.

**Q: Why do LLMs fail at this without an MCP?**
LLMs lack true mathematical persistence. When calculating multi-step proportions (subtotal -> ratio -> tax allocation -> tip allocation -> fractional rounding), they often lose tracking of pennies, resulting in individual totals that don't add up to the receipt's grand total.

**Q: What is the 'Penny Reconciliation Algorithm'?**
Due to floating-point `toFixed(2)` rounding on 5 different people, the sum of individual owed amounts might equal $100.01 while the actual grand total is $100.00. The engine detects this and surgically subtracts or adds the penny discrepancy to guarantee an exact match.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deterministic-fair-share-tip-splitter](https://vinkius.com/mcp/deterministic-fair-share-tip-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deterministic Fair-Share Tip Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `deterministic-fair-share-tip-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deterministic Fair-Share Tip Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deterministic-fair-share-tip-splitter": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
