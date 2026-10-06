# Shower Savings Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/shower-savings-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare the environmental and financial impact of different shower routines.

## Description
This MCP server allows you to evaluate the environmental and economic footprint of your showering habits. By analyzing water consumption and the energy required for heating, you can identify significant savings. Use `analyze_routine` to calculate the impact of a single routine, or `compare_routines` to see the direct difference between two or more setups. You can also use `validate_flow_rate` to check if your showerhead is eco-friendly and `get_household_profile` to load your saved utility rates and household size for consistent results.


## Available Tools (4)
- **get_household_profile**: Retrieves a standardized set of household parameters to ensure consistent comparisons
- **validate_flow_rate**: Verifies if a specific showerhead flow rate is within standard residential or eco-friendly ranges
- **analyze_routine**: Calculates the total water and energy impact of a single shower routine
- **compare_routines**: Evaluates the difference in cost and resource usage between two or more specific routines


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shower Savings Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the impact of a 5-minute shower with a 2.0 L/min flow rate for a family of 4?"

**🤖 AI Agent:**
> A 5-minute shower with a 2.0 L/min flow rate for 4 people results in a weekly water usage of 560 liters and a total weekly cost of $12.45.

---

**👤 You:**
> "Compare a high-flow shower (9.5 L/min) with an eco-friendly shower (5.7 L/min) for a single person."

**🤖 AI Agent:**
> Switching to the eco-friendly shower will save you 3.8 liters of water per shower and reduce your weekly costs by $4.20.

---

**👤 You:**
> "Is a flow rate of 4.5 L/min considered eco-friendly?"

**🤖 AI Agent:**
> Yes, a flow rate of 4.5 L/min is categorized as Eco-Friendly.


## ❓ FAQ

**Q: How do I calculate my potential savings?**
You can use the `compare_routines` tool by providing details for two different shower setups. It will calculate the water and energy saved, as well as the total financial savings.

**Q: Can I check if my showerhead is efficient?**
Yes, use the `validate_flow_rate` tool with your showerhead's flow rate to see if it falls into the High, Standard, or Eco-Friendly category.

**Q: What factors affect the cost calculation?**
The cost is determined by the volume of water used, the price of water, the energy required for heating (based on the temperature delta), and the price of energy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/shower-savings-comparator](https://vinkius.com/en/ai-agent-connect/shower-savings-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shower Savings Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shower-savings-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shower Savings Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shower-savings-comparator": {
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
