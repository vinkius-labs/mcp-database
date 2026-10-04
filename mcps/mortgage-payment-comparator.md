# Mortgage Payment Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/mortgage-payment-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare mortgage scenarios to find the best monthly payment, total interest, or cash to close.

## Description
This MCP server provides a suite of financial tools to evaluate mortgage options. Use `compare_loan_options` to rank multiple scenarios based on your priority, such as lowest monthly cost or least interest paid. You can use `calculate_single_option` for a detailed breakdown of a specific loan, `evaluate_affordability` to check if a loan fits your budget, or `find_optimal_down_payment` to determine how much you need to pay upfront to reach a target monthly payment.


## Available Tools (4)
- **calculate_single_option**: Performs a deep dive into a single mortgage scenario to verify its individual costs
- **compare_loan_options**: Evaluates a set of different mortgage scenarios to identify the best financial fit
- **evaluate_affordability**: Checks if a specific loan option fits within a user's defined monthly budget and liquid cash constraints
- **find_optimal_down_payment**: Determines the necessary down payment required to hit a specific target monthly payment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mortgage Payment Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare these two loans: Option 1 is $400,000 price, $80,000 down, 6% rate, 30 years, $300 taxes, $100 insurance, $50 HOA, $5,000 closing. Option 2 is $400,000 price, $100,000 down, 5.5% rate, 30 years, $300 taxes, $100 insurance, $50 HOA, $5,000 closing. Rank them by monthlyPayment."

**🤖 AI Agent:**
> Option 2 is the better choice for monthly affordability with a payment of $2,115.35, compared to Option 1 which costs $2,415.35.

---

**👤 You:**
> "I want to buy a house for $350,000. I can afford $1,800 a month. The rate is 6.5% for 30 years, with $250 taxes, $150 insurance, and $0 HOA. How much down payment do I need?"

**🤖 AI Agent:**
> To achieve a monthly payment of $1,800, you will need a down payment of $63,452.12.

---

**👤 You:**
> "Calculate the breakdown for a $500,000 home with $50,000 down, 7% interest, 30 years, $400 taxes, $200 insurance, $100 HOA, and $10,000 closing costs."

**🤖 AI Agent:**
> The monthly payment is $3,445.32, the total interest over 30 years is $718,114.80, and your total cash to close is $60,000.00.


## ❓ FAQ

**Q: How can I compare multiple loan offers at once?**
You can use the `compare_loan_options` tool. Simply provide a list of your loan scenarios and specify if you want to rank them by monthly payment, total interest, or cash to close.

**Q: Can I check if a mortgage fits my monthly budget?**
Yes, the `evaluate_affordability` tool allows you to input your maximum monthly budget and available cash to see if a specific loan option is viable.

**Q: How do I calculate the required down payment for a specific monthly target?**
Use the `find_optimal_down_payment` tool. It calculates the necessary upfront amount needed to ensure your monthly payment stays within your desired limit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/mortgage-payment-comparator](https://vinkius.com/en/ai-agent-connect/mortgage-payment-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mortgage Payment Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mortgage-payment-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mortgage Payment Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mortgage-payment-comparator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
