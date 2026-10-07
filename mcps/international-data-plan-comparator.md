# International Data Plan Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/international-data-plan-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare roaming, eSIM, and local SIM options to find the best connectivity for your trip.

## Description
This MCP server acts as a decision-support engine for international travelers. It evaluates connectivity tiers including Roaming, eSIM, and Local SIM based on your specific data needs, trip duration, and functional requirements like hotspot or voice support. Use `compare_connectivity_options` to find the best overall method, `get_plan_details` for specific cost breakdowns, `evaluate_roaming_feasibility` to check if your current carrier is a good deal, or `calculate_cost_per_gb` to identify the most efficient data plans.


## Available Tools (4)
- **evaluate_roaming_feasibility**: Evaluate if using a current home carrier is a viable roaming option
- **get_plan_details**: Get detailed information about a specific connectivity plan
- **calculate_cost_per_gb**: Calculate the cost efficiency of available plans
- **compare_connectivity_options**: Compare different connectivity options based on travel requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **International Data Plan Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which connectivity method is best if I need 10GB of data for a 14-day trip and need a hotspot?"

**🤖 AI Agent:**
> The best option for your 14-day trip with 10GB and hotspot requirements is the eSIM Pro Plan, costing $25.00 total.

---

**👤 You:**
> "Is it worth staying with Verizon for a 7-day trip to France needing 5GB?"

**🤖 AI Agent:**
> No, switching to a local eSIM would save you approximately $30.00 compared to Verizon roaming.

---

**👤 You:**
> "Show me the details for plan ID 'esim_premium_01'."

**🤖 AI Agent:**
> The esim_premium_01 plan costs $45.00 total ($40.00 base + $5.00 activation) and provides 20GB of data for 30 days, including hotspot support.


## ❓ FAQ

**Q: How do I find the best plan for my trip?**
You can use the `compare_connectivity_options` tool by providing your required data volume, trip duration, and whether you need hotspot or voice services.

**Q: Can I check if my current carrier is too expensive?**
Yes, use the `evaluate_roaming_feasibility` tool with your carrier name and destination to see potential savings.

**Q: What is the difference between eSIM and Local SIM?**
eSIM is a digital profile you download, while a Local SIM is a physical card you buy in the destination country. Both are compared using the available tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/international-data-plan-comparator](https://vinkius.com/en/ai-agent-connect/international-data-plan-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **International Data Plan Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `international-data-plan-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **International Data Plan Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "international-data-plan-comparator": {
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
