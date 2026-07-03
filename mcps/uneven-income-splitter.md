# Uneven Income Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uneven-income-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate fair expense sharing based on individual income levels.

## Description
The Uneven Income Splitter MCP server provides tools to distribute bills proportionally rather than equally. By using the `get_propose_split` tool, you can input a total bill and a list of participants with their respective incomes to receive an exact monetary breakdown for each person. The system also includes `calculate_individual_share_percentage` to determine a specific person's weight in the group and `verify_payment_accuracy` to audit payments against expected proportional shares. This ensures financial integrity by handling rounding discrepancies automatically.


## Available Tools (3)
- **calculate_individual_share_percentage**: Determines exactly what percentage of the group's collective responsibility rests on one specific person
- **get_propose_split**: Calculates the exact monetary amount each person owes toward a specific bill
- **verify_payment_accuracy**: Audits a set of provided payments against a known bill amount to ensure they match the proportional logic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Uneven Income Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Split a $1200 rent bill between Alice (income: 5000) and Bob (income: 3000)."

**🤖 AI Agent:**
> Alice owes $750.00 and Bob owes $450.00.

---

**👤 You:**
> "What percentage of the total income does Charlie represent if the group is Charlie (2000), Dave (4000), and Eve (4000)?"

**🤖 AI Agent:**
> Charlie represents 20% of the total group income.

---

**👤 You:**
> "Verify if these payments for a $100 bill are correct: Alice (60) and Bob (40), where Alice earns 60 and Bob earns 40."

**🤖 AI Agent:**
> true


## ❓ FAQ

**Q: How does the splitting logic work?**
The split is calculated by determining each person's income as a percentage of the total group income. The bill is then distributed according to these percentages.

**Q: How are rounding errors handled?**
To ensure the sum of all shares exactly matches the total bill, any one-cent discrepancy is automatically adjusted by adding or removing one cent from the participant with the highest income.

**Q: Can I verify if a payment was correct?**
Yes, you can use the `verify_payment_accuracy` tool to audit provided payments against the expected proportional split.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uneven-income-splitter](https://vinkius.com/mcp/uneven-income-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Uneven Income Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `uneven-income-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Uneven Income Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "uneven-income-splitter": {
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
