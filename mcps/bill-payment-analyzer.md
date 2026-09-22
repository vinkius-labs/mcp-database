# Bill Payment Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bill-payment-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyzes collections of bills to count paid and unpaid statuses and calculate outstanding totals.

## Description
This MCP server provides tools to analyze financial obligations within a list of bill records. It allows AI agents to determine the volume of paid versus outstanding bills using `count_bill_statuses`, calculate the total remaining liability with `get_unpaid_bill_total`, find the percentage of completed payments via `get_payment_completion_rate`, and isolate specific records using `filter_bills_by_status`.


## Available Tools (4)
- **count_bill_statuses**: Counts how many bills are paid and how many are unpaid
- **filter_bills_by_status**: Filters bills by their status (paid or unpaid)
- **get_payment_completion_rate**: Calculates the percentage of bills that have been paid
- **get_unpaid_bill_total**: Calculates the total outstanding amount for all unpaid bills


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bill Payment Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many bills have been paid in this list: [{"amountDue": 100, "amountPaid": 100}, {"amountDue": 50, "amountPaid": 0}]?"

**🤖 AI Agent:**
> There is 1 paid bill and 1 unpaid bill.

---

**👤 You:**
> "What is the total outstanding amount for these bills: [{"amountDue": 200, "amountPaid": 50}, {"amountDue": 100, "amountPaid": 100}]?"

**🤖 AI Agent:**
> The total outstanding amount is 150.

---

**👤 You:**
> "What is the payment completion rate for [{"amountDue": 10, "amountPaid": 10}, {"amountDue": 10, "amountPaid": 10}, {"amountDue": 10, "amountPaid": 0}]?"

**🤖 AI Agent:**
> The payment completion rate is 0.6666666666666666.


## ❓ FAQ

**Q: How is a bill considered 'paid'?**
A bill is classified as paid if the total amount paid is equal to or greater than the amount due.

**Q: Can I see only the bills that are still owed?**
Yes, you can use the `filter_bills_by_status` tool with the status set to 'unpaid' to retrieve those specific records.

**Q: What information do I need to provide?**
You need to provide a JSON-stringified array of bill objects, where each object contains the amount due and the amount paid.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bill-payment-analyzer](https://vinkius.com/en/ai-agent-connect/bill-payment-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bill Payment Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bill-payment-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bill Payment Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bill-payment-analyzer": {
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
