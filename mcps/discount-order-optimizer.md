# Discount Order Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/discount-order-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Find the optimal sequence of multiple discounts to achieve the absolute minimum final price.

## Description
The Discount Order Optimizer is a specialized tool designed to solve the complex problem of sequential discount application. When applying multiple discounts--such as percentage reductions, fixed amounts, and shipping adjustments--the order in which they are applied significantly impacts the final total. This MCP server uses an exhaustive permutation algorithm to evaluate every possible sequence, checking eligibility conditions like minimum spend thresholds at each step. By using tools like `find_optimal_discount_sequence`, `calculate_sequence_impact`, and `validate_discount_eligibility`, you can determine exactly how to structure promotions to maximize savings for your customers or optimize pricing strategies.


## Available Tools (3)
- **calculate_sequence_impact**: Calculates impact of a specific sequence
- **find_optimal_discount_sequence**: Finds the best order of discounts
- **validate_discount_eligibility**: Checks if a single discount is applicable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Discount Order Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the best order for these discounts: $100 total, 10% off, and $5 fixed discount?"

**🤖 AI Agent:**
> The optimal sequence is applying the $5 fixed discount first, then the 10% reduction. This results in a final price of $85.50 (Step 1: $100 - $5 = $95; Step 2: $95 * 0.9 = $85.50).

---

**👤 You:**
> "Calculate the impact of applying a 20% discount followed by a $15 shipping discount on a $50 order."

**🤖 AI Agent:**
> The final price is $25.00. Step-by-step: $50.00 - 20% ($10.00) = $40.00; then $40.00 - $15.00 shipping discount = $25.00.

---

**👤 You:**
> "Is a 15% discount valid for a user with a $30 total if the minimum spend is $40?"

**🤖 AI Agent:**
> No, the discount is not applicable because the current running total of $30 does not meet the required minimum spend threshold of $40.


## ❓ FAQ

**Q: How does the optimization algorithm work?**
The tool generates all possible permutations of your provided discounts. For each sequence, it simulates the application process step-by-step, verifying if conditions like `min_spend` are met at the exact moment each discount is applied. It then returns the sequence that results in the lowest final price.

**Q: Can I check if a specific discount is valid for my current cart total?**
Yes, you can use the `validate_discount_eligibility` tool. By providing the current running total, the discount object, and the user context (like membership tier), the tool will confirm if the discount is applicable or explain why it was skipped.

**Q: Does the tool handle different types of discounts?**
Yes, it supports `percentage` reductions, `fixed_amount` subtractions, and `fixed_shipping` adjustments. The optimizer considers how each type interacts with others in a sequence.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/discount-order-optimizer](https://vinkius.com/mcp/discount-order-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Discount Order Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `discount-order-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Discount Order Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "discount-order-optimizer": {
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
