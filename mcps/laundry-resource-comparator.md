# Laundry Resource Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/laundry-resource-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Analyze and compare water, energy, and detergent usage across different laundry machine settings.

## Description
This MCP server provides tools to evaluate the environmental footprint of laundry operations. Use `get_machine_settings` to find available profiles for front-load, top-load, or industrial machines. You can use `calculate_resource_totals` to project cumulative usage over many cycles, or `compare_settings_efficiency` to determine which setting is better for your specific priority, such as water or energy savings. For advanced scenarios, `evaluate_custom_impact` allows you to adjust detergent amounts or energy multipliers to see how specific changes affect your total resource consumption.


## Available Tools (4)
- **calculate_resource_totals**: Calculates the cumulative water, energy, and detergent usage for a specific setting over a set number of loads
- **compare_settings_efficiency**: Compares two different machine settings to determine which is more resource-efficient based on user-defined priorities
- **evaluate_custom_impact**: Optional: custom detergent amount or energy multiplier.

Allows a user to provide manual adjustments to see how it changes the footprint
- **get_machine_settings**: g., "front_load", "top_load", or "industrial".

Retrieves the available configuration profiles for a specific laundry machine type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Laundry Resource Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the available settings for a front load machine?"

**🤖 AI Agent:**
> The available profiles for a front load machine are Eco, Heavy Duty, and Quick Wash.

---

**👤 You:**
> "Which is more efficient for water usage: Eco or Heavy Duty for 10 loads on a front load machine?"

**🤖 AI Agent:**
> The Eco profile is more efficient, providing a 30% reduction in water usage compared to Heavy Duty over 10 loads.

---

**👤 You:**
> "Calculate the total energy used for 50 cycles of the Eco profile on a front load machine."

**🤖 AI Agent:**
> The total energy used for 50 cycles of the Eco profile is 45.0 kWh.


## ❓ FAQ

**Q: How can I find available washing machine profiles?**
You can use the `get_machine_settings` tool by providing the machine type, such as 'front_load' or 'top_load'.

**Q: Can I compare two different settings directly?**
Yes, the `compare_settings_efficiency` tool allows you to compare two profiles based on a priority factor like water, energy, or detergent.

**Q: How do I account for older, less efficient machines?**
Use the `evaluate_custom_impact` tool and provide an `energyMultiplier` to adjust the energy consumption for your specific machine.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/laundry-resource-comparator](https://vinkius.com/en/ai-agent-connect/laundry-resource-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Laundry Resource Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `laundry-resource-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Laundry Resource Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "laundry-resource-comparator": {
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
