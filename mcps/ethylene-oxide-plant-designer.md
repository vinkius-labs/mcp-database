# Ethylene Oxide Plant Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ethylene-oxide-plant-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Engineering design tool for simulating and sizing Ethylene Oxide production facilities.

## Description
This MCP server provides specialized engineering tools for designing Ethylene Oxide (EO) production plants. It allows engineers to simulate reactor sizing, catalyst requirements, process efficiency, and safety constraints based on feedstock availability and catalyst selection. Use `calculate_reactor_dimensions` to determine vessel size, `estimate_catalyst_requirements` for silver catalyst mass, `analyze_process_efficiency` to predict selectivity, and `generate_safety_envelope` to establish safe operating limits for both air and oxygen-based processes.


## Available Tools (4)
- **analyze_process_efficiency**: Predicts the selectivity and conversion rates for the given inputs
- **calculate_reactor_dimensions**: Determines the physical size and design parameters of the reactor vessel
- **estimate_catalyst_requirements**: Calculates the necessary mass and volume of silver catalyst needed to meet production goals
- **generate_safety_envelope**: Defines the safe operating limits to prevent explosion or thermal runaway


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ethylene Oxide Plant Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the reactor dimensions for 50 units of ethylene using the oxygen process and the standard silver catalyst."

**🤖 AI Agent:**
> The reactor requires a volume of 125.5 m³, a height of 12.0 m, a diameter of 3.6 m, and a heat exchange area of 45.2 m².

---

**👤 You:**
> "How much silver catalyst is needed for an annual capacity of 10,000 tons using the high-activity catalyst?"

**🤖 AI Agent:**
> The required catalyst mass is 4,500 kg with a total volume of 5,200 liters and a loading density of 0.86 kg/L.

---

**👤 You:**
> "What is the expected selectivity for 30 units of ethylene using the air process?"

**🤖 AI Agent:**
> The predicted selectivity is 78.5% with an ethylene conversion rate of 12.2% and a CO2 yield of 21.5%.


## ❓ FAQ

**Q: How do I determine the reactor size?**
You can use the `calculate_reactor_dimensions` tool by providing the ethylene availability, the oxygen source (air or oxygen), and the specific catalyst system.

**Q: What is the difference between the air and oxygen processes?**
The air process uses atmospheric air, which is safer due to lower oxygen concentration but requires larger equipment. The oxygen process uses pure oxygen, allowing for higher throughput and smaller equipment but requires stricter safety controls.

**Q: Can I check the safety limits for my design?**
Yes, use the `generate_safety_envelope` tool to define maximum temperature and oxygen concentration limits to prevent thermal runaway or explosions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ethylene-oxide-plant-designer](https://vinkius.com/en/ai-agent-connect/ethylene-oxide-plant-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ethylene Oxide Plant Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ethylene-oxide-plant-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ethylene Oxide Plant Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ethylene-oxide-plant-designer": {
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
