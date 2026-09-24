# Cancellation Refund Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cancellation-refund-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise refund amounts and penalty breakdowns for bookings.

## Description
This MCP server provides a suite of tools to manage booking cancellations. You can use `calculate_refund_amount` to determine exact payouts, `verify_refund_eligibility` to check if a customer qualifies for a refund, and `generate_refund_summary` for human-readable financial breakdowns. For high-volume reporting, `batch_calculate_refunds` processes multiple scenarios simultaneously.


## Available Tools (4)
- **batch_calculate_refunds**: Processes multiple cancellation scenarios at once for high-volume reporting
- **calculate_refund_amount**: Determines the exact amount of money to be returned to the customer
- **generate_refund_summary**: Provides a human-readable breakdown of the financial transaction
- **verify_refund_eligibility**: Checks if a refund is possible under specific constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cancellation Refund Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the refund for a $200 booking with a 20% cancellation penalty."

**🤖 AI Agent:**
> The refund amount is $160.00, and the penalty amount is $40.00.

---

**👤 You:**
> "Is a customer eligible for a refund if the booking price is $50 and the penalty is 100%?"

**🤖 AI Agent:**
> No, the customer is not eligible for a refund because the cancellation penalty is 100%.

---

**👤 You:**
> "Give me a summary for a $1000 booking with a 15% penalty."

**🤖 AI Agent:**
> The original price was $1000.00, a penalty of $150.00 was applied, and the final amount returned is $850.00.


## ❓ FAQ

**Q: How do I check if a customer is eligible for a refund?**
You can use the `verify_refund_eligibility` tool. It checks if the booking price is valid and if the cancellation penalty is less than 100%.

**Q: Can I process multiple refunds at once?**
Yes, the `batch_calculate_refunds` tool allows you to process an array of multiple cancellation scenarios in a single request.

**Q: What information is needed to calculate a refund?**
To use `calculate_refund_amount`, you need the original booking price and the cancellation percentage penalty.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cancellation-refund-calculator](https://vinkius.com/en/ai-agent-connect/cancellation-refund-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cancellation Refund Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cancellation-refund-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cancellation Refund Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cancellation-refund-calculator": {
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
