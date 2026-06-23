# US Lease Break Penalty Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-lease-break-penalty-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Estimate financial liabilities and settlement ranges for US residential and commercial lease terminations.

## Description
This MCP server provides specialized tools to calculate the financial impact of breaking a lease in the United States. Using `calculate_gross_loss`, you can determine total unpaid rent. With `get_state_mitigation_duty`, agents can retrieve state-specific legal obligations regarding a landlord's duty to mitigate damages. Finally, `estimate_lease_break_settlement` provides a calculated range for a reasonable settlement, accounting for re-letting costs and mitigation factors.


## Available Tools (3)
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


## ❓ FAQ

**Q: How can I calculate the total unpaid rent?**
Use the `calculate_gross_loss` tool by providing the monthly rent and the number of months remaining in the lease term.

**Q: Does this server account for state laws?**
Yes. The `get_state_mitigation_duty` tool provides specific legal mitigation obligations and expected reduction factors based on the provided US state code.

**Q: Can I estimate a final settlement amount?**
Yes. The `estimate_lease_break_settlement` tool calculates a reasonable range for settlement, considering the gross loss, re-letting costs, and state-specific mitigation factors.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-lease-break-penalty-calculator](https://vinkius.com/mcp/us-lease-break-penalty-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Lease Break Penalty Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-lease-break-penalty-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Lease Break Penalty Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-lease-break-penalty-calculator": {
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
