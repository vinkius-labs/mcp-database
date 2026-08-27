# Wine Oxygen Management Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-oxygen-management-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate cumulative oxygen pickup, optimize inert gas usage, and validate closure suitability.

## Description
This MCP server provides precision tools for winemakers to manage dissolved oxygen (DO) throughout the production lifecycle. Use `calculate_cumulative_oxygen_pickup` to predict total oxygen absorption across processing steps like racking or filtration. Optimize gas usage with `recommend_inert_gas_usage` to determine the exact volume of Nitrogen or Argon needed for tank purging. Ensure long-term bottle stability by using `evaluate_closure_suitability` to check if a closure's OTR meets your target exposure limits. Additionally, `analyze_saturation_risk` helps monitor if current DO levels are approaching physical saturation limits based on temperature and pressure.


## Available Tools (4)
- **analyze_saturation_risk**: Analyze the risk of dissolved oxygen saturation
- **calculate_cumulative_oxygen_pickup**: Calculate cumulative oxygen pickup throughout all planned processing steps
- **evaluate_closure_suitability**: Evaluate if a specific bottle closure is suitable for the intended shelf life
- **recommend_inert_gas_usage**: Calculate required inert gas volume to purge a tank


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Oxygen Management Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much total oxygen will my wine absorb if I have 1000L of wine, a 50L headspace, and 5 hours of exposure during racking?"

**🤖 AI Agent:**
> The cumulative oxygen pickup for this step is 0.45 mg/L.

---

**👤 You:**
> "How much Nitrogen do I need to purge a 500L tank with a 40L headspace to reach a target oxygen level of 0.5 mg/L?"

**🤖 AI Agent:**
> You will need 38.5 liters of Nitrogen to achieve the target oxygen level in the headspace.

---

**👤 You:**
> "Is a closure with an OTR of 0.05 cm3/mm*day suitable for a 750ml bottle for 24 months?"

**🤖 AI Agent:**
> Yes, the predicted oxygen pickup is 0.02 mg/L, which is well within your target limits for a 2-year shelf life.


## ❓ FAQ

**Q: How can I predict oxygen pickup during racking?**
You can use the `calculate_cumulative_oxygen_pickup` tool by providing the volume of wine, the headspace volume, and the duration of the racking step.

**Q: How do I know if my cork is suitable for long-term aging?**
Use the `evaluate_closure_suitability` tool. Input the closure's OTR, the bottle volume, and your target maximum pickup to see if it is suitable for your intended shelf life.

**Q: Can I calculate the amount of Argon needed for tank purging?**
Yes, the `recommend_inert_gas_usage` tool calculates the required volume of inert gas based on your tank volume, headspace, and target oxygen level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-oxygen-management-calculator](https://vinkius.com/ai-agent-connect/wine-oxygen-management-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Oxygen Management Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-oxygen-management-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Oxygen Management Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-oxygen-management-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
