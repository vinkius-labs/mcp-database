# INSS Retirement Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/inss-retirement-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Estimate your Brazilian social security retirement benefits based on age, contribution time, and average salary.

## Description
The INSS Retirement Estimator provides precise calculations for potential monthly social security benefits in Brazil. By using tools like `estimate_monthly_benefit`, users can determine their expected payout after applying the current INSS ceiling and transition rules from the recent social security reform. The server also allows you to `list_applicable_transition_rules` to see which legal pathways you are approaching, and `get_pension_reference_values` to check the current maximum (ceiling) and minimum (floor) benefit amounts.


## Available Tools (3)
- **estimate_monthly_benefit**: Estimates the monthly retirement benefit amount
- **get_pension_reference_values**: Retrieves current INSS ceiling and minimum benefit values
- **list_applicable_transition_rules**: Lists retirement rules the user qualifies for or approaches


## 💬 Prompt Examples

Here are some examples of how you can interact with the **INSS Retirement Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will I receive monthly if I am 55 years old, have 30 years of contribution, and an average salary of 4000?"

**🤖 AI Agent:**
> Based on the current rules, your estimated monthly benefit is R$ 3,200.00, applying the transition rule for your profile.

---

**👤 You:**
> "What are the current INSS ceiling and minimum benefit values?"

**🤖 AI Agent:**
> The current maximum monthly benefit (ceiling) is R$ 7,786.02, and the minimum benefit floor is R$ 1,412.00.

---

**👤 You:**
> "Which retirement rules am I approaching with 60 years of age and 35 years of contribution?"

**🤖 AI Agent:**
> You currently satisfy the criteria for the Points System rule, and you are also approaching the Minimum Age transition requirement.


## ❓ FAQ

**Q: How accurate is the retirement estimate?**
The estimate is based on hardcoded transition rules and current INSS reference values. While it provides a highly reliable projection using the Points System and Minimum Age criteria, it should be used for planning purposes rather than as official legal advice.

**Q: What information do I need to provide?**
To use `estimate_monthly_benefit`, you will need your current age, total years of social security contributions, and your average monthly salary throughout your career.

**Q: Can I see which retirement rules apply to me?**
Yes, you can use the `list_applicable_transition_rules` tool to identify which transition pathways, such as the Points System or Minimum Age requirements, you currently satisfy or are approaching.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/inss-retirement-estimator](https://vinkius.com/mcp/inss-retirement-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **INSS Retirement Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `inss-retirement-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **INSS Retirement Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "inss-retirement-estimator": {
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
