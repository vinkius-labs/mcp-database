# Lavender Oil Yield Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/lavender-oil-yield-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Estimate lavender essential oil yield, chemical profiles, and distillation efficiency.

## Description
This MCP server provides specialized tools for lavender cultivation and processing analysis. It allows AI agents to calculate expected oil yield per hectare using `calculate_expected_yield`, predict aromatic compound concentrations like linalool with `estimate_chemical_profile`, and estimate operational needs via `calculate_distillation_efficiency`. Additionally, users can identify the best time for harvest using `get_harvest_recommendation` to ensure maximum oil quality.


## Available Tools (4)
- **calculate_distillation_efficiency**: Estimates the operational requirements for the extraction process
- **calculate_expected_yield**: Determines the total amount of essential oil produced per unit of land
- **estimate_chemical_profile**: Predicts the concentration of key aromatic compounds
- **get_harvest_recommendation**: Identifies the ideal time to harvest for maximum quality


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lavender Oil Yield Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected yield for 5000 kg/ha of Lavandula angustifolia with 2% oil content?"

**🤖 AI Agent:**
> The expected yield for Lavandula angustifolia is 100 kg/ha.

---

**👤 You:**
> "Estimate the distillation requirements for 200kg of biomass using steam distillation."

**🤖 AI Agent:**
> The estimated distillation time is 4.5 hours with an energy requirement of 120 kWh.

---

**👤 You:**
> "What is the chemical profile for Lavandula angustifolia in the Full Bloom stage?"

**🤖 AI Agent:**
> The profile shows a linalool content of 35% and a linalyl acetate content of 25%, resulting in a High quality grade.


## ❓ FAQ

**Q: How do I calculate the expected oil yield?**
Use the `calculate_expected_yield` tool by providing the lavender variety, the biomass per hectare, and the expected oil content percentage.

**Q: Can I predict the quality of the oil?**
Yes, the `estimate_chemical_profile` tool predicts linalool and linalyl acetate levels, which determine the oil's quality grade.

**Q: How can I find the best time to harvest?**
The `get_harvest_recommendation` tool analyzes the specific variety to identify the optimum flower development stage for peak quality.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/lavender-oil-yield-calculator](https://vinkius.com/ai-agent-connect/lavender-oil-yield-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lavender Oil Yield Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lavender-oil-yield-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lavender Oil Yield Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lavender-oil-yield-calculator": {
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
