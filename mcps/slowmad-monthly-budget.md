# Slowmad Monthly Budget MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/slowmad-monthly-budget)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate total trip costs, monthly burn rates, and savings sufficiency for long-term travel.

## Description
Plan your long-term travel with precision. This MCP server provides tools to calculate the complete financial requirements for digital nomads. Use `calculate_trip_budget` to determine your total required funds, including monthly burn rates and upfront costs like visas and insurance. You can also use `compare_city_scenarios` to evaluate different destinations side-by-side, or `calculate_reserve_sufficiency` to check if your current savings can cover your planned journey including a safety buffer. It is designed to help you manage your monthly burn rate and upfront cash requirements for any destination.


## Available Tools (4)
- **calculate_reserve_sufficiency**: Determines if a specific amount of savings is enough to cover a planned trip including the safety buffer
- **calculate_trip_budget**: Calculates the complete financial requirement for a single destination over a specific duration
- **compare_city_scenarios**: Compares the total cost and monthly burn rate of multiple destination profiles
- **get_monthly_breakdown**: Provides a granular view of how the monthly burn rate is distributed across different categories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Slowmad Monthly Budget** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the budget for a 6-month stay in Lisbon with 1500 rent, 300 utilities, 400 food, 100 transport, 100 coworking, 200 recreation, and a 20% reserve."

**🤖 AI Agent:**
> For a 6-month stay in Lisbon, your monthly burn rate is 2600. Your total required funds, including a 20% reserve, is 18200.

---

**👤 You:**
> "I have 5000 in savings. Is this enough for a trip that requires 4500 total funds?"

**🤖 AI Agent:**
> Yes, your savings are sufficient to cover the planned trip.

---

**👤 You:**
> "Show me the monthly breakdown for a budget with 1200 rent, 200 utilities, 300 food, 50 transport, 50 coworking, and 100 recreation."

**🤖 AI Agent:**
> Your monthly burn rate is 1900. The breakdown is: Rent: 1200, Utilities: 200, Food: 300, Transport: 50, Coworking: 50, Recreation: 100.


## ❓ FAQ

**Q: How do I calculate my total trip cost?**
You can use the `calculate_trip_budget` tool. Provide your stay duration, monthly costs for rent, food, and utilities, as well as any one-time upfront fees like visas.

**Q: Can I compare different cities?**
Yes, the `compare_city_scenarios` tool allows you to input multiple destination profiles to see which one is the most affordable based on total funds and monthly burn rate.

**Q: How is the safety buffer calculated?**
The reserve amount is calculated by multiplying your monthly burn rate by the reserve percentage you provide, then multiplying that by your total stay duration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/slowmad-monthly-budget](https://vinkius.com/en/ai-agent-connect/slowmad-monthly-budget)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Slowmad Monthly Budget** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `slowmad-monthly-budget` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Slowmad Monthly Budget** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "slowmad-monthly-budget": {
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
