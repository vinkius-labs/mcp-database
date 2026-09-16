# Oil Tanker Voyage Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/oil-tanker-voyage-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Calculate voyage duration, fuel consumption, and maritime profitability.

## Description
This MCP server provides essential tools for maritime logistics and oil tanker operations. It allows AI agents to perform complex voyage calculations, including `calculate_voyage_metrics` for economic summaries, `analyze_canal_impact` for transit delays, `evaluate_demurrage_risk` for port penalty assessments, and `validate_port_accessibility` to ensure vessel safety based on draft and berth availability.

### Available Tools

`calculate_voyage_metrics_tool`, `analyze_canal_impact_tool`, `evaluate_demurrage_risk_tool`, `validate_port_accessibility_tool`


## Available Tools (4)
- **analyze_canal_impact_tool**: Evaluates the time and cost penalties associated with passing through specific canals
- **calculate_voyage_metrics_tool**: Provides the core economic and temporal summary of a proposed voyage
- **evaluate_demurrage_risk_tool**: Calculates potential financial penalties based on port stay durations
- **validate_port_accessibility_tool**: Determines if a vessel can safely enter a specific port based on physical constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Oil Tanker Voyage Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the metrics for a voyage of 5000 nautical miles with a cargo of 100000 units, traveling at 14 knots, with a fuel rate of 50 per hour and a freight rate of 20 per unit."

**🤖 AI Agent:**
> The voyage will take approximately 357.14 hours, consume 17857.14 units of fuel, generate 2000000 in total freight revenue, and result in an estimated voyage cost of 2742857.14.

---

**👤 You:**
> "Will a vessel with a draft of 18 meters be able to enter a port with a maximum draft of 17.5 meters and an available berth?"

**🤖 AI Agent:**
> No, the vessel cannot enter the port because its draft exceeds the maximum allowed depth.

---

**👤 You:**
> "Calculate the demurrage penalty if the actual port stay was 48 hours, the allowed laytime was 36 hours, and the demurrage rate is 5000 per hour."

**🤖 AI Agent:**
> The total demurrage penalty incurred is 60000.


## ❓ FAQ

**Q: How can I check if my vessel can enter a specific port?**
You can use the `validate_port_accessibility` tool by providing the vessel draft, the port's maximum draft, and berth availability. Tools available: `calculate_voyage_metrics_tool`, `analyze_canal_impact_tool`, `evaluate_demurrage_risk_tool`.

**Q: Can this tool help with fuel cost estimation?**
Yes, the `calculate_voyage_metrics` tool calculates total fuel consumed based on distance, speed, and the fuel consumption rate.

**Q: How are canal delays handled?**
The `analyze_canal_impact` tool evaluates the total delay hours and transit fees associated with specific canal routes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/oil-tanker-voyage-planner](https://vinkius.com/en/ai-agent-connect/oil-tanker-voyage-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Oil Tanker Voyage Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `oil-tanker-voyage-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Oil Tanker Voyage Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "oil-tanker-voyage-planner": {
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
