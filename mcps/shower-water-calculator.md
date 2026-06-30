# Shower Water Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shower-water-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate water usage, costs, and carbon emissions for showers.

## Description
The Shower Water Calculator MCP server allows AI agents to calculate the environmental and financial impact of shower sessions. Using tools like `calculate_consumption`, `estimate_cost`, `calculate_emissions`, and `get_shower_summary`, users can determine total liters used, compare duration against the UN 5-minute sustainability benchmark, estimate utility costs, and quantify carbon footprints (CO2e). This server acts as a bridge for AI clients like Cursor, VS Code, Claude Desktop, and Windsurf to access precise resource consumption data.


## Available Tools (4)
- **estimate_cost**: Estimate the cost of water usage
- **calculate_consumption**: Calculate water consumption and benchmark status
- **calculate_emissions**: Estimate carbon emissions from water usage
- **get_shower_summary**: Get a comprehensive shower usage report


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shower Water Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much water did I use in a 10-minute shower with a flow rate of 9 liters per minute?"

**🤖 AI Agent:**
> You used 90 liters of water. Since the duration was 10 minutes, it exceeded the UN 5-minute sustainability benchmark.

---

**👤 You:**
> "What is the estimated cost for 150 liters of water if the price is $0.002 per liter?"

**🤖 AI Agent:**
> The total cost for 150 liters at $0.002 per liter is $0.30.

---

**👤 You:**
> "Calculate the carbon footprint for 100 liters of water with an emission factor of 0.5g/L."

**🤖 AI Agent:**
> The estimated carbon footprint is 50 grams of CO2e.


## ❓ FAQ

**Q: What does `calculate_consumption` do?**
It calculates the total liters of water used based on flow rate and duration, and checks if you met the UN 5-minute benchmark.

**Q: How can I see all my data in one view?**
Use the `get_shower_summary` tool to receive a unified report containing consumption, cost, and emissions.

**Q: Does this tool estimate financial costs?**
Yes, the `estimate_cost` tool calculates the monetary expense based on the volume of water used and your local unit price.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shower-water-calculator](https://vinkius.com/mcp/shower-water-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shower Water Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shower-water-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shower Water Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shower-water-calculator": {
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
