# Foil Pump Efficiency Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/foil-pump-efficiency-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Calculate hydrofoil pumping energy, speed gain, and efficiency.

## Description
This MCP server provides specialized calculation tools for hydrofoil riders to analyze their pumping performance. Use `get_pump_energy` to determine the work performed per stroke, `calculate_speed_gain` to estimate velocity increases, and `evaluate_pumping_efficiency` to assess overall energy conversion. For a complete data snapshot, use `get_performance_summary` to retrieve energy, speed, and efficiency metrics in one call.


## Available Tools (4)
- **evaluate_pumping_efficiency**: Calculates the overall efficiency percentage of the pumping session
- **get_performance_summary**: Provides a comprehensive overview of the pumping profile
- **get_pump_energy**: Calculates the work performed during a single pumping stroke
- **calculate_speed_gain**: Determines the theoretical increase in forward velocity resulting from one pump cycle


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Foil Pump Efficiency Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much energy is generated per pump for a 75kg rider with a 90cm mast?"

**🤖 AI Agent:**
> The energy generated per pump is 735.75 Joules.

---

**👤 You:**
> "What is the speed gain for a wing with 1200cm² area, 80cm mast, and 5 aspect ratio?"

**🤖 AI Agent:**
> The theoretical speed gain per pump is 0.45 m/s.

---

**👤 You:**
> "Calculate the efficiency for a 70kg rider, 1100cm² wing, 0.6 aspect ratio, 40 pumps per minute, and 0.8 technique."

**🤖 AI Agent:**
> The overall pumping efficiency is 62.5%.


## ❓ FAQ

**Q: How do I calculate the energy used in one pump?**
You can use the `get_pump_energy` tool by providing the rider's weight in kilograms and the mast length in centimeters.

**Q: What factors influence the speed gain?**
Speed gain is determined by the wing area, the mast length, and the wing's aspect ratio via the `calculate_speed_gain` tool.

**Q: Can I get a full performance report?**
Yes, the `get_performance_summary` tool provides a complete overview including energy per pump, speed gain, and efficiency percentage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/foil-pump-efficiency-engine](https://vinkius.com/en/ai-agent-connect/foil-pump-efficiency-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Foil Pump Efficiency Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `foil-pump-efficiency-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Foil Pump Efficiency Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "foil-pump-efficiency-engine": {
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
