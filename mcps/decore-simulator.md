# DECORE Simulator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/decore-simulator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate and validate income declarations for regulatory compliance.

## Description
The DECORE Simulator is a specialized financial engine designed to help users verify the compliance of their income declarations. By using tools like `calculate_total_monthly_revenue`, `validate_income_compliance`, and `compute_taxable_burden`, you can accurately aggregate different revenue streams--including Pro-labore, Profit Distribution, and Autonomous income--and determine if they fall within safe regulatory thresholds or require additional documentation.


## Available Tools (3)
- **validate_income_compliance**: Validate if income amounts are within regulatory boundaries
- **calculate_total_monthly_revenue**: Calculate total monthly revenue and its composition
- **compute_taxable_burden**: Calculate the portion of total income subject to tax


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DECORE Simulator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my total revenue with 5000 pro-labore, 2000 distribution, and 1000 autonomous income."

**🤖 AI Agent:**
> Your total monthly revenue is 8000. The composition is 62.5% Pro-labore, 25% Profit Distribution, and 12.5% Autonomous income.

---

**👤 You:**
> "Check if my income of 10000 pro-labore is compliant."

**🤖 AI Agent:**
> The status is Critical because the Pro-labore amount exceeds the allowed threshold.

---

**👤 You:**
> "How much of my 5000 total income is taxable?"

**🤖 AI Agent:**
> The taxable portion of your income is 5000, while the exempt portion is 0.


## ❓ FAQ

**Q: What does the simulator calculate?**
It calculates total monthly revenue, checks if your income amounts are within regulatory compliance limits using `validate_income_compliance`, and estimates your taxable burden.

**Q: How do I know if my income is in a 'Warning' state?**
A 'Warning' status is triggered when any of your income categories reach 80% of their predefined regulatory threshold.

**Q: Does the tool handle different types of income?**
Yes, it specifically processes Pro-labore, Profit Distribution, and Autonomous income streams.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/decore-simulator](https://vinkius.com/mcp/decore-simulator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DECORE Simulator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `decore-simulator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DECORE Simulator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "decore-simulator": {
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
