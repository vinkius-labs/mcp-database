# Commission Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/commission-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate and summarize commission amounts and agent earnings.

## Description
This MCP server provides tools to manage and analyze commission data. You can use `get_total_commission` to sum up a list of amounts, `filter_commissions_by_type` to isolate specific transaction categories, and `get_commission_summary_by_agent` to see a detailed breakdown of earnings for a specific agent. It also includes `validate_commission_entry` to ensure all financial entries meet business requirements.


## Available Tools (4)
- **get_commission_summary_by_agent**: Provides a breakdown of total commissions earned by a specific agent across different transaction types
- **get_total_commission**: Calculates the sum of all commission amounts provided in a list
- **validate_commission_entry**: Checks if a single commission entry meets all business requirements for validity
- **filter_commissions_by_type**: Filters a list of commission entries to only include those matching a specific transaction category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Commission Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total sum of these commissions: 150.50, 200.00, and 50.25?"

**🤖 AI Agent:**
> The total sum of the commissions is 400.75.

---

**👤 You:**
> "Show me the commission summary for agent 'A123'."

**🤖 AI Agent:**
> Agent A123 has earned a total of 1250.00, with 800.00 from Retail and 450.00 from Wholesale.

---

**👤 You:**
> "Filter the commissions to only show 'Service' types."

**🤖 AI Agent:**
> The filtered commissions for 'Service' are: 100.00, 250.00, and 75.00.


## ❓ FAQ

**Q: How do I sum multiple commissions?**
You can use the `get_total_commission` tool by providing a list of commission amounts.

**Q: Can I see a breakdown of earnings by transaction type?**
Yes, the `get_commission_summary_by_agent` tool provides both the total amount and a breakdown by transaction type for a specific agent.

**Q: How can I verify if a commission entry is valid?**
Use the `validate_commission_entry` tool to check if an entry has a positive amount, a valid agent ID, and a valid type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/commission-total](https://vinkius.com/en/ai-agent-connect/commission-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Commission Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `commission-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Commission Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "commission-total": {
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
