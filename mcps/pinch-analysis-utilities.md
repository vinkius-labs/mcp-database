# Pinch Analysis Utilities MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/pinch-analysis-utilities)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Thermodynamic target calculation and heat recovery optimization using pinch technology.

## Description
This MCP server provides a suite of tools for chemical engineering pinch analysis. It allows agents to calculate fundamental thermodynamic targets, evaluate the impact of stream splitting, validate heat exchanger network designs for violations, and optimize utility costs. Use `analyze_pinch_targets` to find the pinch point and minimum utility requirements, or `check_pinch_violation` to ensure your design respects the minimum approach temperature.


## Available Tools (4)
- **analyze_pinch_targets**: 
- **calculate_utility_optimization**: 
- **check_pinch_violation**: 
- **evaluate_stream_splitting**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pinch Analysis Utilities** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the pinch targets for a process with these hot streams: [{'supplyTemp': 150, 'targetTemp': 50, 'heatCapacityFlowRate': 10}] and cold streams: [{'supplyTemp': 30, 'targetTemp': 120, 'heatCapacityFlowRate': 8}] with a min approach temp of 10."

**🤖 AI Agent:**
> The pinch temperature is 40°C, with a minimum hot utility of 120 kW and a minimum cold utility of 45 kW.

---

**👤 You:**
> "Check if this design violates pinch rules: hot streams: [{'supplyTemp': 100, 'targetTemp': 40, 'heatCapacityFlowRate': 5}], cold streams: [{'supplyTemp': 50, 'targetTemp': 90, 'heatCapacityFlowRate': 5}], heat exchangers: [{'hotStreamId': 'h1', 'coldStreamId': 'c1', 'duty': 200}], utilities: [], minApproachTemp: 10."

**🤖 AI Agent:**
> No violation detected. The design satisfies the minimum approach temperature constraint.

---

**👤 You:**
> "What happens if I split a hot stream with ID 'H1' by a ratio of 0.5?"

**🤖 AI Agent:**
> Splitting stream H1 with a 0.5 ratio increases the maximum heat recovery by 15% and reduces the required hot utility by 10 kW.


## ❓ FAQ

**Q: How do I find the minimum utility requirements?**
You can use the `analyze_pinch_targets` tool to calculate the minimum hot and cold utility requirements based on your stream data and minimum approach temperature.

**Q: Can I check if my heat exchanger network is valid?**
Yes, the `check_pinch_violation` tool validates whether your design violates pinch rules or the minimum approach temperature constraint.

**Q: Does this tool support stream splitting analysis?**
Yes, use `evaluate_stream_splitting` to determine if dividing a stream's flow rate improves heat recovery or satisfies temperature constraints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/pinch-analysis-utilities](https://vinkius.com/ai-agent-connect/pinch-analysis-utilities)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pinch Analysis Utilities** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pinch-analysis-utilities` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pinch Analysis Utilities** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pinch-analysis-utilities": {
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
