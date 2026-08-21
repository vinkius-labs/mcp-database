# CPF Optimization Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/cpf-optimization-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic CPF allocation and projection engine for Singaporeans aged 20-35.

## Description
This MCP server provides precise financial planning tools for Singaporeans aged 20-35 to optimize their Central Provident Fund (CPF) allocations. By using `calculate_cpf_strategy`, users can receive a monthly contribution breakdown tailored to specific life goals like BTO housing, retirement, or balanced investment. The engine also provides 10-year interest projections and calculates BTO readiness based on current OA balances. You can also use `get_cpf_interest_rates` to verify the deterministic rates applied to OA, SA, and MA accounts, or `validate_contribution_limits` to ensure proposed allocations remain within statutory bounds.


## Available Tools (3)
- **calculate_cpf_strategy**: Generates a monthly contribution breakdown and financial projections based on a user's age, income, and primary life goal
- **get_cpf_interest_rates**: Retrieves the current deterministic interest rates used for all CPF calculations
- **validate_contribution_limits**: Ensures that the proposed monthly contributions do not exceed statutory or logical limits for the user's age group


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CPF Optimization Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am 25 years old, earn 4000 SGD monthly, have 20000 in OA, 10000 in SA, and 5000 in MA. I want to save for a BTO priced at 500000. What is my strategy?"

**🤖 AI Agent:**
> Based on your goal for BTO, your recommended monthly contributions are OA: 1200 SGD, SA: 300 SGD, and MA: 200 SGD. Your current BTO readiness is 4.0%.

---

**👤 You:**
> "I am 30 years old, earn 5000 SGD monthly, with 50000 in OA, 20000 in SA, and 10000 in MA. I want to focus on retirement. How much tax relief can I get?"

**🤖 AI Agent:**
> For your retirement goal, the recommended voluntary top-up to maximize tax relief is 8000 SGD.

---

**👤 You:**
> "What are the current CPF interest rates?"

**🤖 AI Agent:**
> The current deterministic interest rates are: OA: 2.5%, SA: 4.0%, and MA: 4.0%.


## ❓ FAQ

**Q: How do I calculate my BTO readiness?**
You can use the `calculate_cpf_strategy` tool and provide an `estimatedBtoPrice`. The tool will return a `btoReadinessPercent` indicating how much of the estimated cost is covered by your current OA balance.

**Q: Can I get tax relief through this tool?**
Yes. If you set your goal to 'retirement', the `calculate_cpf_strategy` tool calculates the `taxReliefEligible` amount, recommending a voluntary top-up to maximize your SGD 8,000 tax deduction limit.

**Q: What interest rates are used for projections?**
The engine uses deterministic rates: 2.5% for the Ordinary Account (OA) and 4% for both the Special Account (SA) and MediSave Account (MA). You can verify these using `get_cpf_interest_rates`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/cpf-optimization-strategy](https://vinkius.com/ai-agent-connect/cpf-optimization-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CPF Optimization Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cpf-optimization-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CPF Optimization Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cpf-optimization-strategy": {
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
