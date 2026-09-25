# Care Recurring Payment Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-recurring-payment-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage recurring bill schedules, responsibility matrices, and automated alert workflows.

## Description
This MCP server provides a financial planning engine to manage recurring obligations. It allows AI agents to generate a chronological `get_payment_calendar`, map responsibilities via `get_owner_matrix`, track notification timelines with `get_alert_schedule`, and identify issues using `get_exception_report`. It applies user-defined due-date buffers and approval thresholds to ensure timely payments and oversight.


## Available Tools (4)
- **get_alert_schedule**: Identifies when notifications must be sent to owners to ensure timely payment
- **get_exception_report**: Lists necessary actions for payments that have hit constraints
- **get_owner_matrix**: Provides a summary of responsibilities to ensure oversight alignment
- **get_payment_calendar**: Generates a chronological schedule of all upcoming payments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Recurring Payment Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all upcoming payments for the next 30 days."

**🤖 AI Agent:**
> Here is your payment schedule for the next 30 days: Rent is due on Oct 1st ($1200), Internet is due on Oct 5th ($60), and Electricity is due on Oct 12th ($150).

---

**👤 You:**
> "Are there any payment issues I need to address right now?"

**🤖 AI Agent:**
> Yes, there is one critical exception: The utility bill for $450 exceeded the approval threshold and requires secondary authorization.

---

**👤 You:**
> "What is the responsibility matrix for John Doe?"

**🤖 AI Agent:**
> John Doe is responsible for the Rent and Insurance bills, using the Primary Checking and Savings accounts.


## ❓ FAQ

**Q: How does the payment calendar handle due dates?**
The `get_payment_calendar` tool calculates effective payment dates by applying a user-defined due-date buffer before the actual due date.

**Q: What happens if a payment exceeds the approval threshold?**
If a payment exceeds the threshold, it triggers an exception that can be identified using `get_exception_report`.

**Q: Can I see which person is responsible for a specific bill?**
Yes, you can use `get_owner_matrix` to view the mapping of owners to their assigned bills and funding sources.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-recurring-payment-calendar](https://vinkius.com/en/ai-agent-connect/care-recurring-payment-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Recurring Payment Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-recurring-payment-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Recurring Payment Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-recurring-payment-calendar": {
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
