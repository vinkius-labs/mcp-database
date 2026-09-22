# Invoice Aging Days MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/invoice-aging-days)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Track and categorize outstanding invoice age for cash flow management.

## Description
This MCP server provides essential tools for financial monitoring and debt collection. It allows AI agents to calculate exactly how many days an invoice has been outstanding using `get_invoice_age`, assign invoices to risk-based categories with `categorize_invoice_bucket`, and generate high-level exposure reports via `get_aging_summary`. It also includes `validate_invoice_data` to ensure batch records are complete and accurate for aging analysis.


## Available Tools (4)
- **validate_invoice_data**: Validate batch
- **categorize_invoice_bucket**: Assign bucket to invoice
- **get_aging_summary**: Summarize exposure
- **get_invoice_age**: Calculate days since invoice date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Invoice Aging Days** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many days old is the invoice issued on 2024-01-01?"

**🤖 AI Agent:**
> The invoice issued on 2024-01-01 is 435 days old.

---

**👤 You:**
> "What category does a 45-day old invoice fall into?"

**🤖 AI Agent:**
> An invoice that is 45 days old falls into the Mid Stage category.

---

**👤 You:**
> "Summarize these invoices: [{'amount': 100, 'daysOld': 10}, {'amount': 200, 'daysOld': 45}]"

**🤖 AI Agent:**
> The summary is: Early Stage: 100, Mid Stage: 200.


## ❓ FAQ

**Q: How do I calculate the age of a specific invoice?**
You can use the `get_invoice_age` tool by providing the invoice date in ISO 8601 format.

**Q: Can I get a summary of all my overdue amounts?**
Yes, the `get_aging_summary` tool aggregates invoice amounts into specific aging buckets to show your total exposure.

**Q: What are the aging buckets used?**
Invoices are categorized into Current, Early Stage, Mid Stage, Late Stage, and Critical based on the number of days they have been outstanding.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/invoice-aging-days](https://vinkius.com/en/ai-agent-connect/invoice-aging-days)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Invoice Aging Days** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `invoice-aging-days` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Invoice Aging Days** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "invoice-aging-days": {
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
