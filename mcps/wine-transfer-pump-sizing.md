# Wine Transfer Pump Sizing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-transfer-pump-sizing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate pump requirements and transfer logistics for moving wine through piping systems.

## Description
This MCP server provides specialized tools for winery operations to calculate the technical requirements for liquid transfers. It accounts for variables like elevation change, hose diameter, and wine viscosity to determine the necessary pump head. Users can use `calculate_pump_requirements` to find the total pressure needed, `compare_hose_efficiency` to evaluate different hose sizes, `estimate_transfer_time` for duration predictions, and `validate_setup_feasibility` to ensure a specific pump can handle the planned transfer.


## Available Tools (4)
- **calculate_pump_requirements**: Determines the total pressure (head) needed and the estimated duration for a transfer
- **compare_hose_efficiency**: Evaluates how different hose diameters impact the required pump power
- **estimate_transfer_time**: Provides a quick estimate of time based on known flow rates and volume
- **validate_setup_feasibility**: Checks if a specific pump's rated head and flow are sufficient


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Transfer Pump Sizing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to move 5000 liters of wine through 50 meters of 30mm hose with a 5 meter elevation gain. The viscosity is 15 cP and it is finished wine. How much pump head do I need?"

**🤖 AI Agent:**
> The total head required for this transfer is 12.4 meters, with an estimated transfer time of 45 minutes at your target flow rate.

---

**👤 You:**
> "Will a pump with 20 meters of max head and 100 L/min max flow work for a 30 meter transfer, 10 meter lift, 25mm hose, 20 cP viscosity, and 50 L/min target flow?"

**🤖 AI Agent:**
> Yes, the setup is feasible. You have a head margin of 4.5 meters and a flow margin of 50 L/min.

---

**👤 You:**
> "How long will it take to transfer 2000 liters at a rate of 40 liters per minute?"

**🤖 AI Agent:**
> The transfer will take 50 minutes.


## ❓ FAQ

**Q: How does viscosity affect my pump requirements?**
Higher viscosity, such as in unfermented must, increases friction loss. You can use `calculate_pump_requirements` to see how this affects the total head required.

**Q: Can I check if my current pump is strong enough for a transfer?**
Yes, use the `validate_setup_feasibility` tool. Input your pump's maximum head and flow rate along with your transfer parameters to check if the setup is feasible.

**Q: How do I estimate how long a tank transfer will take?**
You can use `estimate_transfer_time` by providing the total volume of wine and the pump's flow rate to get a duration in minutes and hours.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-transfer-pump-sizing](https://vinkius.com/en/ai-agent-connect/wine-transfer-pump-sizing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Transfer Pump Sizing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-transfer-pump-sizing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Transfer Pump Sizing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-transfer-pump-sizing": {
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
