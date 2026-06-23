# UK Statutory Interest Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uk-statutory-interest-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate statutory interest and fixed compensation for late commercial payments in the UK.

## Description
This MCP server provides tools to determine recoverable costs under the UK's Late Payment of Commercial Debts Act 1998. It calculates statutory interest (Bank of England base rate + 8%) and fixed compensation fees based on debt magnitude. Use `total_claim_summary` for a complete breakdown of interest, compensation, and total claim value.


## Available Tools (3)
- **compensation_fee**: Calculate the fixed compensation fee
- **total_claim_summary**: Calculate a full summary of the claim
- **accrued_interest**: Calculate statutory interest accrued on a debt


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UK Statutory Interest Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total claim for a debt of £500 that was due on 2024-01-01."

**🤖 AI Agent:**
> The total claim value is £535.42, which includes £35.42 in accumulated interest and a £40 fixed compensation fee.

---

**👤 You:**
> "How much compensation is owed for an unpaid invoice of £15,000?"

**🤖 AI Agent:**
> The fixed statutory compensation amount for a debt of £15,000 is £100.

---

**👤 You:**
> "Show me the interest accrued on £2,000 since 2023-06-01."

**🤖 AI Agent:**
> The total interest accumulated since 2023-06-01 on a debt of £2,000 is £142.50.


## ❓ FAQ

**Q: How is the interest rate calculated?**
The rate is determined by taking the Bank of England base rate applicable during each period and adding a fixed margin of 8%.

**Q: What is the compensation fee?**
The fixed compensation amount depends on the debt size: £40 for debts up to £1,000, £70 for debts up to £10,000, and £100 for anything above.

**Q: Which tool should I use for a full breakdown?**
You should use the `total_claim_summary` tool to get the interest, compensation, and total claim value in one response.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uk-statutory-interest-calculator](https://vinkius.com/mcp/uk-statutory-interest-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UK Statutory Interest Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `uk-statutory-interest-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UK Statutory Interest Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "uk-statutory-interest-calculator": {
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
