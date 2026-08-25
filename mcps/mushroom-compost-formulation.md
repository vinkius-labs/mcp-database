# Mushroom Compost Formulation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mushroom-compost-formulation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate precise material proportions, hydration, and nitrogen levels for mushroom compost substrates.

## Description
This MCP server provides specialized tools for mushroom compost production. It uses least-cost optimization to determine the exact quantities of carbon and nitrogen sources needed to reach a target C:N ratio. Users can use `calculate_substrate_mix` to find the ideal material proportions and water requirements, `predict_compost_lifecycle` to estimate the duration of Phase I and Phase II composting stages, and `validate_material_safety` to ensure the mix is not toxic to mushroom mycelium.


## Available Tools (3)
- **predict_compost_lifecycle**: Estimates the time required to complete the biological phases of composting based on environmental conditions
- **validate_material_safety**: Checks if a proposed material mix contains any elements or ratios that would be toxic to mushroom mycelium
- **calculate_substrate_mix**: Determines the exact quantities of available raw materials needed to meet a specific target C:N ratio and moisture level at the lowest possible cost


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mushroom Compost Formulation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a substrate mix for 1000kg of compost with a 17:1 C:N ratio and 65% moisture using straw and poultry litter."

**🤖 AI Agent:**
> To produce 1000kg of compost at a 17:1 C:N ratio, you need 845kg of straw and 120kg of poultry litter, plus 35kg of water addition.

---

**👤 You:**
> "How long will it take for my compost pile to finish Phase I if the initial temperature is 25°C and the ambient temperature is 20°C?"

**🤖 AI Agent:**
> Phase I is estimated to last 5 days, and Phase II is estimated to last 12 days, with a total completion date of 2024-06-20.

---

**👤 You:**
> "Is a mix of 90% straw and 10% poultry litter safe for mushrooms without gypsum?"

**🤖 AI Agent:**
> The mix is flagged as unsafe because it lacks gypsum for structural stability in a high-litter substrate.


## ❓ FAQ

**Q: How do I calculate the right mix for my compost?**
You can use the `calculate_substrate_mix` tool by providing your available materials, target C:N ratio, and desired moisture level.

**Q: Can I predict how long the composting process will take?**
Yes, the `predict_compost_lifecycle` tool estimates the duration of both Phase I and Phase II based on temperature and pile volume.

**Q: How do I know if my substrate is safe for mushrooms?**
Use the `validate_material_safety` tool to check if your material mix contains toxic nitrogen levels or lacks necessary structural conditioners.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mushroom-compost-formulation](https://vinkius.com/ai-agent-connect/mushroom-compost-formulation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mushroom Compost Formulation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mushroom-compost-formulation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mushroom Compost Formulation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mushroom-compost-formulation": {
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
