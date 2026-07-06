# Early Lease Break Penalty Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/early-lease-break-penalty-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate the total financial cost of breaking a lease early.

## Description
This MCP server provides tools to determine the total move-out cost when terminating a rental agreement before its scheduled end date. It parses complex text-based penalty clauses (e.g., '2 months rent + 50% of one month') and calculates both the contractual penalty fee and any applicable prorated rent for the final partial month of occupancy. Use `calculate_total_break_cost` to get an aggregated breakdown of all costs, or `parse_penalty_logic` to decompose a clause into numerical components.


## Available Tools (3)
- **calculate_prorated_rent**: Calculate prorated rent for the final month
- **calculate_total_break_cost**: Calculate the total cost to break a lease
- **parse_penalty_logic**: Parse a lease penalty clause


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Early Lease Break Penalty Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will it cost to break my lease if my rent is $2,000 and the clause says '2 months rent'?"

**🤖 AI Agent:**
> The contractual penalty is $4,000. If you have no prorated rent for the final month, your total move-out cost is $4,000.

---

**👤 You:**
> "Calculate my lease break cost: $1,500 rent, 3 months left, clause is '1 month rent + 50% of one month', and I am leaving on the 15th of a 30-day month."

**🤖 AI Agent:**
> The total move-out cost is $2,250. This includes a $2,250 penalty component and $750 prorated rent component.

---

**👤 You:**
> "What is the base multiplier for a clause that says '1.5 months rent'?"

**🤖 AI Agent:**
> The extracted base multiplier is 1.5 months.


## ❓ FAQ

**Q: What inputs are required for the calculation?**
You need to provide the monthly rent amount, the number of months remaining on your lease, and the text from your penalty clause.

**Q: Can I parse complex penalty clauses?**
Yes, the `parse_penalty_logic` tool is designed to extract multipliers and percentages from text like '1 month rent + 50% of one month'.

**Q: Does it account for prorated rent?**
Yes, if you provide the departure day and total days in the month, `calculate_prorated_rent` will determine the portion of rent owed for that final partial month.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/early-lease-break-penalty-calculator](https://vinkius.com/mcp/early-lease-break-penalty-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Early Lease Break Penalty Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `early-lease-break-penalty-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Early Lease Break Penalty Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "early-lease-break-penalty-calculator": {
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
