# Cloud Storage Plan Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cloud-storage-plan-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Compare cloud storage plans by cost, capacity, and usage efficiency.

## Description
This MCP server provides a decision-support engine to evaluate and rank cloud storage subscriptions. It calculates the true monthly equivalent cost, identifies capacity headroom, and predicts overage penalties. Use `compare_plans` to find the best value across multiple tiers, `calculate_plan_efficiency` to assess a single plan against your current data footprint, or `get_overage_projection` to estimate future costs if your usage grows. It helps you avoid overpaying for unused space or facing unexpected overage fees.


## Available Tools (4)
- **get_plan_details**: Retrieves the specific details of a single storage plan
- **calculate_plan_efficiency**: Determines the financial and capacity efficiency of a plan relative to a user's current needs
- **compare_plans**: Ranks multiple plans to find the optimal choice based on cost and capacity
- **get_overage_projection**: Predicts the total cost if a user exceeds their plan capacity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cloud Storage Plan Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which of these plans is the best value for 500GB of usage: plan_standard_500 or plan_premium_1000?"

**🤖 AI Agent:**
> The `plan_premium_1000` is the best value choice, providing a monthly equivalent cost of $8.50 with 500GB of headroom.

---

**👤 You:**
> "How much will it cost if I use 120GB on a 100GB plan?"

**🤖 AI Agent:**
> The total projected cost for 120GB on that plan is $15.00, which includes the base fee and a $5.00 overage penalty.

---

**👤 You:**
> "Check the efficiency of plan_basic_250 for my current 200GB usage."

**🤖 AI Agent:**
> The `plan_basic_250` has a monthly cost of $4.99, provides 50GB of capacity headroom, and carries no overage risk.


## ❓ FAQ

**Q: How does the tool calculate the best value plan?**
The `compare_plans` tool ranks plans primarily by their monthly equivalent cost. If two plans have the same cost, it uses capacity headroom as a tie-breaker to favor the plan that provides more space without excessive waste.

**Q: Can I predict costs for future data growth?**
Yes, you can use `get_overage_projection` to estimate the total cost if your projected data usage exceeds the capacity of a specific plan.

**Q: What is the difference between monthly and annual costs?**
The engine calculates the monthly equivalent cost. For annual plans, it divides the total annual price by twelve to provide a fair comparison against monthly-only plans.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cloud-storage-plan-comparator](https://vinkius.com/en/ai-agent-connect/cloud-storage-plan-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cloud Storage Plan Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cloud-storage-plan-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cloud Storage Plan Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cloud-storage-plan-comparator": {
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
