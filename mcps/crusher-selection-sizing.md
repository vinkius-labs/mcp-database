# Crusher Selection & Sizing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/crusher-selection-sizing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Select optimal crusher types and calculate sizing, power, and wear requirements.

## Description
This MCP server provides specialized engineering tools for mining and aggregate processing. It allows AI agents to determine the most suitable crusher type--such as jaw, gyratory, cone, or impact--based on material hardness and abrasiveness. Beyond selection, it calculates physical dimensions, estimates electrical power demand, and predicts maintenance needs due to material wear using tools like `select_crusher_type`, `calculate_crusher_dimensions`, `estimate_power_demand`, and `calculate_wear_impact`.


## Available Tools (4)
- **estimate_power_demand**: Calculates the energy required to operate the crusher
- **calculate_crusher_dimensions**: Estimates the physical size and capacity of the selected crusher
- **calculate_wear_impact**: Predicts the impact of material abrasiveness on equipment maintenance and efficiency
- **select_crusher_type**: Determines the most suitable category of crusher based on material hardness, abrasiveness, and required reduction ratio


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crusher Selection & Sizing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What type of crusher should I use for hard, abrasive material with a 500mm feed size?"

**🤖 AI Agent:**
> For hard and abrasive material with a 500mm feed size, a Jaw crusher is the most suitable primary crushing option.

---

**👤 You:**
> "Calculate the power needed for a cone crusher processing 200 tons per hour of hard material with a 4:1 reduction ratio."

**🤖 AI Agent:**
> The estimated power requirement for this cone crusher operation is 350 KW, with a peak load of 410 KW.

---

**👤 You:**
> "What are the dimensions for a jaw crusher with a throughput of 150 tons per hour and 400mm feed size?"

**🤖 AI Agent:**
> The jaw crusher will have an opening width of 850mm, a crushing gap of 120mm, and an estimated weight of 12,500 kg.


## ❓ FAQ

**Q: How do I choose between a jaw and a gyratory crusher?**
You can use the `select_crusher_type` tool. It evaluates material hardness, abrasiveness, and feed size to recommend the best primary crusher for your operation.

**Q: Can I estimate the electricity needed for my equipment?**
Yes, the `estimate_power_demand` tool calculates the required power in KW based on the crusher type, throughput, and material hardness.

**Q: How does material abrasiveness affect my maintenance?**
The `calculate_wear_impact` tool predicts the wear life estimate and maintenance frequency by analyzing the material's abrasiveness and the throughput rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/crusher-selection-sizing](https://vinkius.com/en/ai-agent-connect/crusher-selection-sizing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crusher Selection & Sizing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crusher-selection-sizing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crusher Selection & Sizing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crusher-selection-sizing": {
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
