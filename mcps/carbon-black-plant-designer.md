# Carbon Black Plant Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/carbon-black-plant-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design furnace black production plants by calculating reactor, quench, and collection system specifications.

## Description
This MCP server provides engineering tools for designing carbon black production facilities using the furnace black process. It allows AI agents to calculate critical parameters for the entire production chain. Use `get_reactor_specifications` to determine furnace dimensions and thermal profiles, `get_quench_system_design` to size cooling equipment, and `get_collection_system_requirements` to define filtration hardware. Finally, use `get_plant_summary` to verify the feasibility and complexity of the complete plant design based on feedstock, capacity, and product grade.


## Available Tools (4)
- **get_plant_summary**: Provides a consolidated overview of the entire plant design
- **get_quench_system_design**: Calculates the cooling requirements and equipment scale for the quench stage
- **get_reactor_specifications**: Determines the necessary dimensions and thermal parameters for the primary reaction furnace
- **get_collection_system_requirements**: Defines the filtration and separation hardware needed to recover the product


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Carbon Black Plant Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Design a plant using oil feedstock with a capacity of 5000 units for grade N330."

**🤖 AI Agent:**
> The design for an N330 grade plant using oil feedstock at 5000 units capacity requires a reactor volume of 450m³, an operating temperature of 1650°C, and a spray-type quench system with a flow rate of 1200 L/min.

---

**👤 You:**
> "What are the filtration requirements for N660 grade at 2000 capacity?"

**🤖 AI Agent:**
> For N660 grade at 2000 capacity, the required filter surface area is 850m², with an expected collection efficiency of 99.2% and a system pressure drop of 15 kPa.

---

**👤 You:**
> "Is it feasible to design a gas-based plant for N550 with 10000 capacity?"

**🤖 AI Agent:**
> The design is feasible. The total estimated equipment mass is 12500kg with a design complexity score of 7.5/10.


## ❓ FAQ

**Q: What parameters are required for a plant design?**
You must provide the feedstock type (e.g., tar, oil, gas), the target production capacity, and the specific carbon black product grade (e.g., N330, N550).

**Q: Can I check if my design is physically possible?**
Yes, by using the `get_plant_summary` tool, the system evaluates if the reactor and quench systems can be scaled to meet your specific capacity and grade requirements.

**Q: How does the tool handle different product grades?**
The tools adjust calculations for reactor residence time, quench cooling rates, and filter surface area based on the specific particle morphology requirements of the chosen grade.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/carbon-black-plant-designer](https://vinkius.com/en/ai-agent-connect/carbon-black-plant-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Carbon Black Plant Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `carbon-black-plant-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Carbon Black Plant Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "carbon-black-plant-designer": {
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
