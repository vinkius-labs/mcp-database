# Plant Population Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plant-population-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate seed density and evaluate planting success against industry standards.

## Description
This MCP server provides precision agriculture tools to calculate plant density. Use `calculate_linear_density` to find plants per meter, `calculate_hectare_density` to compute theoretical and real populations per hectare based on germination rates, and `evaluate_population_status` to compare your results against soybean and corn benchmarks.


## Available Tools (3)
- **calculate_hectare_density**: Calculate theoretical and real population per hectare
- **calculate_linear_density**: Calculate plants per meter based on plant spacing
- **evaluate_population_status**: Evaluate if planting density is within recommended range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plant Population Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many plants are in one meter if the spacing is 20cm?"

**🤖 AI Agent:**
> With a spacing of 20cm, there are 5 plants per meter.

---

**👤 You:**
> "Calculate the real population for corn with 70cm row spacing, 15cm plant spacing, and 90% germination."

**🤖 AI Agent:**
> The theoretical population is 95,238 plants/ha and the real population is 85,714 plants/ha.

---

**👤 You:**
> "Is a soybean population of 400,000 plants/ha good?"

**🤖 AI Agent:**
> No, a population of 400,000 plants/ha is Above Target for soybean.


## ❓ FAQ

**Q: How do I calculate plants per meter?**
Use the `calculate_linear_density` tool by providing the distance between individual seeds in centimeters.

**Q: Can I account for germination failure?**
Yes, use `calculate_hectare_density` and provide the expected germination rate percentage to see both theoretical and real populations.

**Q: How does the tool evaluate crop health?**
The `evaluate_population_status` tool compares your calculated population against hardcoded benchmarks for soybean and corn to determine if it is optimal, below target, or above target.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plant-population-calculator](https://vinkius.com/mcp/plant-population-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plant Population Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `plant-population-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plant Population Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plant-population-calculator": {
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
