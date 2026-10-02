# Family Phone Plan Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-phone-plan-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare multi-line mobile plans to find the lowest total cost of ownership.

## Description
This MCP server provides tools to calculate and compare the total cost of ownership for multi-line mobile phone plans. It accounts for service fees, data usage overages, device installments, and regional taxes. Use `compare_plans` to evaluate multiple options at once, or `calculate_total_account_cost` to get a detailed breakdown of monthly and annual expenses for a specific plan.


## Available Tools (4)
- **calculate_total_account_cost**: Aggregates service costs, hardware installments, and taxes to find the complete monthly and annual cost for a household
- **compare_plans**: Evaluates multiple plans against a specific household profile to find the cheapest option
- **get_plan_details**: Retrieves the base configuration and pricing rules for a specific mobile plan
- **calculate_line_costs**: Calculates the monthly service cost for a single line based on its data usage and the selected plan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Phone Plan Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which plan is cheapest for 4 lines with 10GB usage each and $20 monthly device costs per line at 7% tax?"

**🤖 AI Agent:**
> The Family Tier plan is the cheapest option, with a total monthly cost of $145.20.

---

**👤 You:**
> "Compare the costs for 2 lines using 50GB of data each."

**🤖 AI Agent:**
> The Unlimited Tier plan is the best fit for high data usage, costing $95.00 per month.

---

**👤 You:**
> "What is the total annual cost for a 3-line plan with $0 device installments and 5% tax?"

**🤖 AI Agent:**
> The total annual cost for this configuration is $420.00.


## ❓ FAQ

**Q: How does the tool calculate the total cost?**
The tool aggregates base service fees, multi-line discounts, data overage charges, monthly hardware installments, and local taxes to provide a complete monthly and annual total.

**Q: Can I compare multiple plans at once?**
Yes, you can use the `compare_plans` tool to evaluate a list of plan IDs against your specific household usage and hardware needs.

**Q: Does this include device costs?**
Yes, the tool includes monthly device installments in the total cost of ownership calculation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-phone-plan-comparator](https://vinkius.com/en/ai-agent-connect/family-phone-plan-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Phone Plan Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-phone-plan-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Phone Plan Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-phone-plan-comparator": {
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
