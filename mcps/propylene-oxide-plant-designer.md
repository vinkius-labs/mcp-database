# Propylene Oxide Plant Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/propylene-oxide-plant-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Engineering tool for designing Propylene Oxide production plants and calculating yields.

## Description
This MCP server provides specialized engineering tools for designing industrial Propylene Oxide (PO) production plants. It allows users to model reactor configurations using `calculate_reactor_design`, determine oxidant needs with `estimate_peroxide_requirements`, and predict secondary product outputs via `calculate_byproduct_yields`. Additionally, it evaluates financial feasibility through `calculate_economic_impact`, accounting for co-product credits and waste management costs across CHPO, PO/TBA, and PO/SM technologies.


## Available Tools (4)
- **calculate_byproduct_yields**: Predicts the mass of secondary products and waste generated during the process
- **calculate_economic_impact**: Calculates the net cost impact by factoring in co-product credits and waste treatment expenses
- **calculate_reactor_design**: Determines the physical dimensions and required volume of the primary reactor based on capacity and technology
- **estimate_peroxide_requirements**: Calculates the amount of oxidant/peroxide needed to support the target production capacity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Propylene Oxide Plant Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the required reactor volume for a 100,000 mtpa plant using PO/SM technology?"

**🤖 AI Agent:**
> The required reactor volume for a 100,000 mtpa PO/SM plant is 450 cubic meters with a residence time of 4.5 hours.

---

**👤 You:**
> "How much styrene will be produced by a 50,000 mtpa PO/SM plant?"

**🤖 AI Agent:**
> A 50,000 mtpa PO/SM plant will produce 35,000 metric tons of styrene annually.

---

**👤 You:**
> "Calculate the economic impact for a 200,000 mtpa CHPO plant with a waste treatment cost of 50 per ton."

**🤖 AI Agent:**
> The net plant impact for this CHPO plant is -15,000,000 due to high waste treatment costs and zero co-product credit.


## ❓ FAQ

**Q: Which production technologies are supported?**
The tool supports three primary technologies: CHPO (Chlorohydrin Process), PO/TBA (Propylene Oxide / Tert-Butyl Alcohol), and PO/SM (Propylene Oxide / Styrene Monomer).

**Q: How can I calculate the reactor volume?**
You can use the `calculate_reactor_design` tool by providing the target annual capacity and the chosen production technology.

**Q: Does the tool account for waste treatment costs?**
Yes, the `calculate_economic_impact` tool factors in the cost to treat one metric ton of waste to determine the net plant impact.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/propylene-oxide-plant-designer](https://vinkius.com/en/ai-agent-connect/propylene-oxide-plant-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Propylene Oxide Plant Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `propylene-oxide-plant-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Propylene Oxide Plant Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "propylene-oxide-plant-designer": {
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
