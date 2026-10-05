# Phone Upgrade Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/phone-upgrade-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze the total cost of ownership for smartphone upgrades.

## Description
This MCP server provides tools to calculate the long-term economic value of smartphone upgrades. It analyzes total cost of ownership (TCO) by factoring in device price, trade-in values, monthly service plans, storage upgrades, and potential repair costs. Use `calculate_device_ownership_cost` to find the annualized cost of a specific device, `compare_upgrade_scenarios` to decide between two different paths, `evaluate_trade_in_efficiency` to check if a trade-in beats a private sale, and `project_repair_risk` to estimate future maintenance expenses.


## Available Tools (4)
- **compare_upgrade_scenarios**: Compares two different upgrade paths to find the most economical choice
- **evaluate_trade_in_efficiency**: Determines if a trade-in is financially beneficial compared to selling a device privately or keeping it
- **project_repair_risk**: Estimates the likelihood and cost impact of repairs based on the device age and usage
- **calculate_device_ownership_cost**: Calculates the total expenditure for a single device configuration over its expected lifespan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Phone Upgrade Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the annualized cost of a $999 phone with a $50 monthly plan used for 3 years?"

**🤖 AI Agent:**
> The annualized cost for this configuration is $416.00 per year.

---

**👤 You:**
> "Should I trade in my phone for $300 or sell it privately for $350 with $20 in shipping costs?"

**🤖 AI Agent:**
> A private sale is recommended as it yields a net gain of $330, which is higher than the $300 trade-in value.

---

**👤 You:**
> "Compare a $800 phone used for 2 years vs a $1200 phone used for 4 years, both with $40 monthly plans."

**🤖 AI Agent:**
> The $1200 phone used for 4 years is the winner with a lower annualized cost.


## ❓ FAQ

**Q: How is the annualized cost calculated?**
The annualized cost is the total lifetime cost (including device price, plans, and repairs) divided by the number of years you plan to keep the device.

**Q: Can I compare financing vs. paying upfront?**
Yes, you can use `compare_upgrade_scenarios` to evaluate different financing options against full upfront payments.

**Q: Does this account for repair costs?**
Yes, you can use `project_repair_risk` to estimate the impact of potential repairs on your total expenditure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/phone-upgrade-comparator](https://vinkius.com/en/ai-agent-connect/phone-upgrade-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Phone Upgrade Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `phone-upgrade-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Phone Upgrade Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "phone-upgrade-comparator": {
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
