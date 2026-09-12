# Synthetic Rubber Plant Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/synthetic-rubber-plant-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Engineering tools for designing synthetic rubber production facilities.

## Description
This MCP server provides a suite of chemical engineering tools to design synthetic rubber production plants. It enables precise calculation of reactor parameters using `calculate_reactor_specs`, determines requirements for solidifying polymer emulsions with `design_coagulation_system`, and estimates final stage scales via `estimate_finishing_requirements`. Additionally, users can validate feedstock availability for specific production targets using `check_monomer_feasibility`.


## Available Tools (4)
- **calculate_reactor_specs**: Determines the required physical parameters for the polymerization reactor
- **check_monomer_feasibility**: Validates if the available feedstock is sufficient to meet the design capacity
- **design_coagulation_system**: Determines the requirements for converting liquid emulsion into solid rubber crumbs
- **estimate_finishing_requirements**: Calculates the scale of the final drying, stripping, and pelletizing stages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Synthetic Rubber Plant Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the reactor specs for an SBR plant with a target capacity of 5000 metric tons using the cold emulsion process."

**🤖 AI Agent:**
> The required reactor volume is 450 m³, with a residence time of 120 minutes and a heat removal requirement of 15.5 MW.

---

**👤 You:**
> "What are the finishing requirements for an NBR plant producing 2000 metric tons with a residual monomer target of 10 ppm?"

**🤖 AI Agent:**
> The stripping column height required is 18 meters, with a drying energy requirement of 4.2 GJ/ton and a pelletizer throughput of 2.5 tons/hour.

---

**👤 You:**
> "Is it feasible to produce 3000 metric tons of SBR if I have 2500 units of styrene and 2000 units of butadiene available?"

**🤖 AI Agent:**
> No, the production is not feasible. The limiting monomer is styrene, resulting in a deficit of 500 units for the target capacity.


## ❓ FAQ

**Q: Which rubber types are supported?**
The server supports SBR (Styrene-Butadiene Rubber), BR (Butadiene Rubber), and NBR (Nitrile Butadiene Rubber).

**Q: Can I model cold emulsion SBR processes?**
Yes, by using `calculate_reactor_specs` and setting the `isColdProcess` parameter to true, the tool adjusts heat removal and residence time for cold emulsion kinetics.

**Q: How do I check if I have enough monomers for my plant?**
You can use the `check_monomer_feasibility` tool by providing the rubber type, target capacity, and a map of your available monomer masses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/synthetic-rubber-plant-designer](https://vinkius.com/en/ai-agent-connect/synthetic-rubber-plant-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Synthetic Rubber Plant Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `synthetic-rubber-plant-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Synthetic Rubber Plant Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "synthetic-rubber-plant-designer": {
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
