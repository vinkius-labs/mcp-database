# Ventilation Fan Sizing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ventilation-fan-sizing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculates ventilation fan requirements and inlet needs for livestock buildings.

## Description
This MCP server provides specialized engineering calculations for livestock ventilation systems. It uses ASABE standards to determine total airflow requirements based on animal species and count. Users can determine the optimal number and size of fans using `calculate_fan_configuration`, calculate necessary inlet areas with `estimate_inlet_requirements` to prevent drafts, and create progressive operation sequences with `generate_fan_staging_schedule`. It ensures precise control over building environments for swine, poultry, and cattle.


## Available Tools (4)
- **get_total_ventilation_requirement**: Determines the total cubic feet per minute (CFM) needed for the building
- **calculate_fan_configuration**: Determines the number and specific sizes of fans required to meet the ventilation target
- **estimate_inlet_requirements**: Calculates the necessary inlet area to prevent excessive air velocity
- **generate_fan_staging_schedule**: Creates a sequence for turning fans on and off to maintain precise airflow control


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ventilation Fan Sizing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total ventilation requirement for 500 swine?"

**🤖 AI Agent:**
> The total ventilation requirement for 500 swine is 25,000 CFM based on standard ASABE rates.

---

**👤 You:**
> "Calculate the fan configuration for 15,000 CFM at 0.1 inches of static pressure using these fans: [{"size": "36in", "capacity": 5000}, {"size": "48in", "capacity": 10000}]"

**🤖 AI Agent:**
> To meet 15,000 CFM, you should install one 48-inch fan and two 36-inch fans, providing a total capacity of 20,000 CFM.

---

**👤 You:**
> "Generate a 3-stage staging schedule for 3 selected fans."

**🤖 AI Agent:**
> Stage 1: 1 fan running (5,000 CFM). Stage 2: 2 fans running (10,000 CFM). Stage 3: 3 fans running (15,000 CFM).


## ❓ FAQ

**Q: How does this tool determine the required airflow?**
The `get_total_ventilation_requirement` tool calculates the total CFM by applying ASABE standard ventilation rates to the specific animal type and count provided.

**Q: Can I customize the ventilation rate?**
Yes, when using `get_total_ventilation_requirement`, you can provide a custom minimum ventilation rate to override the standard ASABE values.

**Q: How do I prevent high air velocity at the inlets?**
You can use `estimate_inlet_requirements` to calculate the necessary inlet area required to keep air velocity below your specified maximum limit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ventilation-fan-sizing](https://vinkius.com/ai-agent-connect/ventilation-fan-sizing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ventilation Fan Sizing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ventilation-fan-sizing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ventilation Fan Sizing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ventilation-fan-sizing": {
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
