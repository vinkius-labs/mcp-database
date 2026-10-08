# Wellness Retreat Budget Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wellness-retreat-budget-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate comprehensive wellness retreat costs including logistics, operations, and overhead.

## Description
This MCP server provides a complete financial planning suite for organizing wellness retreats. It allows AI agents to calculate precise budgets by breaking down costs into core logistics, operational services, wellness add-ons, and financial overhead. Use `calculate_base_logistics` to handle housing and travel, `calculate_operational_costs` for meals and classes, and `calculate_wellness_and_overhead` for treatments and taxes. Finally, use `generate_final_budget` to aggregate all figures into a complete group and per-person financial summary with a safety contingency.


## Available Tools (4)
- **generate_final_budget**: Aggregates all cost categories into the final group and per-person summaries
- **calculate_base_logistics**: Calculates the primary costs related to housing and travel for the group
- **calculate_operational_costs**: Calculates the costs associated with food and scheduled activities
- **calculate_wellness_and_overhead**: Calculates the costs for specialized treatments and government/administrative obligations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wellness Retreat Budget Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the base logistics for a retreat with 20 people, where lodging is $150 per person and total transport is $2000."

**🤖 AI Agent:**
> The total lodging cost is $3,000 and the transport cost is $2,000, resulting in a base logistics total of $5,000. The per-person logistics cost is $250.

---

**👤 You:**
> "What are the operational costs for 10 participants if meals are $50 per person and classes cost $500 in total?"

**🤖 AI Agent:**
> The total meal cost is $500 and the class cost is $500, making the operational total $1,000. The per-person operational cost is $100.

---

**👤 You:**
> "I have a subtotal of $5000. Calculate the overhead if treatments cost $1000, taxes are 10%, and service fees are $200."

**🤖 AI Agent:**
> The treatment cost is $1,000, the tax total is $500, and the service fees are $200, resulting in an overhead total of $1,700.


## ❓ FAQ

**Q: How do I calculate the total cost for my retreat?**
You can use `generate_final_budget` to aggregate all your calculated costs into a single total, which includes a contingency buffer for unforeseen expenses.

**Q: Can I include taxes and service fees in the budget?**
Yes, the `calculate_wellness_and_overhead` tool is specifically designed to include treatment costs, tax percentages, and service fees.

**Q: Does this tool account for the number of participants?**
Yes, most tools require the `participantCount` to accurately calculate per-person costs and total lodging or meal expenses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wellness-retreat-budget-planner](https://vinkius.com/en/ai-agent-connect/wellness-retreat-budget-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wellness Retreat Budget Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wellness-retreat-budget-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wellness Retreat Budget Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wellness-retreat-budget-planner": {
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
