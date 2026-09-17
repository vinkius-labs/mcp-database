# Topping Wine Requirement Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/topping-wine-requirement-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate wine replenishment needs for barrel aging based on evaporation and environment.

## Description
This MCP server provides tools to manage the 'Angel's Share' during wine aging. It calculates the volume of wine lost to evaporation by accounting for barrel age and cellar humidity. Use `get_monthly_topping_volume` to find monthly losses, `get_total_topping_requirement` for the full aging period, `get_topping_schedule` to plan replenishment events, and `get_allocation_strategy` to manage reserve wine stocks.


## Available Tools (4)
- **get_allocation_strategy**: Recommends how much of the reserve wine stock should be set aside for topping
- **get_monthly_topping_volume**: Calculates how much wine is expected to be lost to evaporation on a monthly basis
- **get_topping_schedule**: Provides a timeline of when topping events should occur based on a specific frequency
- **get_total_topping_requirement**: Determines the total volume of wine needed to cover the entire aging period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Topping Wine Requirement Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much wine will I need for 50 barrels over 24 months with a 2% evaporation rate and 70% humidity?"

**🤖 AI Agent:**
> You will need a total of 120 liters of wine to cover the 24-month aging period for 50 barrels.

---

**👤 You:**
> "What is the monthly loss for 10 barrels with 3% evaporation and 50% humidity?"

**🤖 AI Agent:**
> The total monthly volume lost for 10 barrels is 2.5 liters.

---

**👤 You:**
> "Give me a topping schedule for 20 barrels every 3 months for a year."

**🤖 AI Agent:**
> Topping events are scheduled for month 3, 6, 9, and 12, with volumes adjusted for cumulative evaporation.


## ❓ FAQ

**Q: How does humidity affect the calculation?**
Lower humidity increases the evaporation rate, requiring more topping wine. The `get_monthly_topping_volume` tool adjusts for this automatically.

**Q: Can I plan my replenishment schedule?**
Yes, use the `get_topping_schedule` tool to generate a timeline of specific months and volumes needed for topping.

**Q: What is the difference between conservative and aggressive strategies?**
A conservative strategy increases the reserve allocation to protect against humidity drops, while an aggressive strategy uses the minimum required volume.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/topping-wine-requirement-calculator](https://vinkius.com/en/ai-agent-connect/topping-wine-requirement-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Topping Wine Requirement Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `topping-wine-requirement-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Topping Wine Requirement Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "topping-wine-requirement-calculator": {
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
