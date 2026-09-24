# Insurance Daily Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/insurance-daily-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate the daily cost of travel insurance policies.

## Description
This MCP server provides tools to analyze travel insurance costs. Use `get_daily_cost` to find the daily burn rate, `get_premium_breakdown` for a detailed view of the premium, `validate_coverage_duration` to check if a trip length is valid, and `compare_policy_affordability` to determine which policy offers better value per day.


## Available Tools (4)
- **compare_policy_affordability**: Compares the daily cost of two different insurance policies to determine which is more cost-effective per day
- **get_daily_cost**: Calculates the cost of insurance for a single day based on the total premium and the number of days covered
- **get_premium_breakdown**: Provides a detailed breakdown of the total premium, showing how much is allocated to the daily cost and how much remains in total
- **validate_coverage_duration**: Checks if a requested number of travel days is compatible with existing premium structures or logical constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Insurance Daily Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the daily cost for a $500 premium covering 20 days?"

**🤖 AI Agent:**
> The daily cost for this insurance policy is $25.00.

---

**👤 You:**
> "Which is cheaper: a $300 premium for 10 days or a $400 premium for 20 days?"

**🤖 AI Agent:**
> The second policy ($400 for 20 days) is cheaper, costing $20.00 per day compared to $30.00 per day for the first policy.

---

**👤 You:**
> "Show me the breakdown for a $1000 premium over 50 days."

**🤖 AI Agent:**
> The daily cost is $20.00, and the remaining balance after one day is $980.00.


## ❓ FAQ

**Q: How do I calculate the daily cost of my insurance?**
You can use the `get_daily_cost` tool by providing the total premium and the number of covered days.

**Q: Can I compare two different insurance policies?**
Yes, use the `compare_policy_affordability` tool to see which policy is more cost-effective per day.

**Q: How do I check if my coverage duration is valid?**
Use the `validate_coverage_duration` tool to verify if your requested days meet the policy requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/insurance-daily-cost-calculator](https://vinkius.com/en/ai-agent-connect/insurance-daily-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Insurance Daily Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `insurance-daily-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Insurance Daily Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "insurance-daily-cost-calculator": {
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
