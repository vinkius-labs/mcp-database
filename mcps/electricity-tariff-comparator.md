# Electricity Tariff Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/electricity-tariff-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare electricity plans by analyzing fixed fees, tiered rates, and time-of-use schedules.

## Description
This MCP server provides tools to analyze and compare electricity service plans. It accounts for fixed monthly fees, tiered consumption rates, and Time-of-Use (ToU) schedules. Users can use `compare_tariffs` to see side-by-side costs for different plans based on their specific consumption profile, or `simulate_usage_impact` to predict how shifting energy usage from peak to off-peak hours affects their total bill. It also allows for detailed inspection of individual plan structures via `get_plan_details` and viewing all available options with `list_available_plans`.


## Available Tools (4)
- **get_plan_details**: Retrieves the complete structure and pricing rules of a specific electricity plan
- **list_available_plans**: Provides a list of all electricity plans currently available
- **simulate_usage_impact**: Answers how changing a user's behavior would affect their total bill under a specific plan
- **compare_tariffs**: Provides a side-by-side comparison of multiple electricity plans


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Electricity Tariff Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare plan_a and plan_b for 500kWh monthly usage with 70% peak and 30% off-peak usage, including a 5% tax."

**🤖 AI Agent:**
> Plan A will cost $55.25 per month, while Plan B will cost $48.50 per month for your specific usage profile.

---

**👤 You:**
> "What happens to my bill if I move 20% of my usage from peak to off-peak hours for plan_c?"

**🤖 AI Agent:**
> Shifting 20% of your usage to off-peak hours will reduce your monthly bill by $12.40.

---

**👤 You:**
> "List all the available electricity plans."

**🤖 AI Agent:**
> The available plans are: Standard Plan A (Fixed), Dynamic Plan B (ToU), and Eco-Saver Plan C (Tiered).


## ❓ FAQ

**Q: How can I compare multiple electricity plans at once?**
You can use the `compare_tariffs` tool by providing the IDs of the plans you want to compare, your total monthly usage in kWh, and your consumption profile.

**Q: Can I see how shifting my usage to off-peak hours saves money?**
Yes, the `simulate_usage_impact` tool is designed specifically to calculate the cost difference when you change your consumption distribution between peak and off-peak periods.

**Q: What information is included in the plan details?**
By using `get_plan_details`, you can retrieve the full pricing structure, including fixed fees, tiered rates, and time-of-use schedules for a specific plan.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/electricity-tariff-comparator](https://vinkius.com/en/ai-agent-connect/electricity-tariff-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Electricity Tariff Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `electricity-tariff-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Electricity Tariff Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "electricity-tariff-comparator": {
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
