# Linear Alkylbenzene (LAB) Plant Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/linear-alkylbenzene-lab-plant-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Engineering tool for modeling LAB production from kerosene and benzene.

## Description
This MCP server provides specialized engineering tools to design and model a Linear Alkylbenzene (LAB) production plant. It allows for precise calculation of feedstock requirements using `calculate_feedstock_requirements`, sizing of the dehydrogenation unit via `size_dehydrogenation_unit`, and modeling of the alkylation reactor with `design_alkylation_reactor`. Finally, users can assess the entire system's performance using `evaluate_plant_yield`. It supports both HF and solid catalyst modeling to ensure accurate plant design.


## Available Tools (4)
- **calculate_feedstock_requirements**: Determines the necessary amounts of benzene and kerosene to meet a specific target LAB production capacity
- **design_alkylation_reactor**: Models the physical requirements of the alkylation reactor based on the chosen catalyst
- **evaluate_plant_yield**: Calculates the final mass of LAB produced and assesses the efficiency of the entire plant design
- **size_dehydrogenation_unit**: Determines the capacity of the dehydrogenation unit needed to prepare the kerosene feed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Linear Alkylbenzene (LAB) Plant Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much benzene and kerosene do I need for a 50,000 ton LAB capacity with a 0.9 yield?"

**🤖 AI Agent:**
> To achieve a 50,000 ton capacity with a 0.9 yield, you require 55,555.56 tons of total feedstock, consisting of the calculated benzene and kerosene amounts.

---

**👤 You:**
> "What is the reactor volume needed for a kerosene feedrate of 100 with a benzene feedrate of 50 using a solid catalyst at 150 degrees?"

**🤖 AI Agent:**
> The required reactor volume is 450 cubic meters with a residence time of 4.5 hours.

---

**👤 You:**
> "Calculate the dehydrogenation unit capacity for a kerosene feedrate of 200 and 0.85 conversion efficiency."

**🤖 AI Agent:**
> The required unit capacity is 200 units, with 30 units of unconverted alkanes remaining.


## ❓ FAQ

**Q: What kind of catalyst models are supported?**
The server supports modeling for both HF (Hydrogen Fluoride) and solid acid catalysts through the `design_alkylation_reactor` tool.

**Q: How do I calculate the necessary benzene and kerosene amounts?**
You can use the `calculate_feedstock_requirements` tool by providing your target LAB capacity and the desired process yield.

**Q: Can I evaluate the total plant efficiency?**
Yes, the `evaluate_plant_yield` tool calculates the final LAB mass, process efficiency, and byproduct mass based on your input parameters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/linear-alkylbenzene-lab-plant-designer](https://vinkius.com/en/ai-agent-connect/linear-alkylbenzene-lab-plant-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Linear Alkylbenzene (LAB) Plant Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `linear-alkylbenzene-lab-plant-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Linear Alkylbenzene (LAB) Plant Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "linear-alkylbenzene-lab-plant-designer": {
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
