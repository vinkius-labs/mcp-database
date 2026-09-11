# Bond Work Index Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bond-work-index-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate Bond Work Index (BWi), grinding energy requirements, and circuit power.

## Description
This MCP server provides specialized tools for mineral processing engineers to perform comminution calculations. Use `calculate_bond_work_index` to determine the material resistance from test data, `estimate_grinding_energy` to predict energy needs for specific size reductions, and `project_circuit_power` to calculate total mill power requirements based on throughput. It also includes `validate_test_data` to ensure input parameters are physically plausible.


## Available Tools (4)
- **calculate_bond_work_index**: Determines the specific Bond Work Index of a material based on experimental test results
- **estimate_grinding_energy**: Predicts the energy needed to grind a specific material to a target size
- **project_circuit_power**: Calculates the total required power for a grinding circuit based on material throughput
- **validate_test_data**: Checks the integrity of grinding test input parameters before calculation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bond Work Index Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Bond Work Index for a test where the feed size is 2500 micrometers, the product size is 150 micrometers, and 12 kWh/t was consumed."

**🤖 AI Agent:**
> The calculated Bond Work Index is 13.45 and the size reduction ratio is 16.67.

---

**👤 You:**
> "Estimate the energy needed to grind material with a BWi of 14 to a product size of 75 micrometers from a feed of 2000 micrometers using dry grinding."

**🤖 AI Agent:**
> The estimated specific energy requirement for dry grinding is 15.22 kWh/t.

---

**👤 You:**
> "What is the required power for a circuit with a specific energy requirement of 10 kWh/t and a throughput of 500 t/h?"

**🤖 AI Agent:**
> The required power is 5000 kW (or 5.0 MW).


## ❓ FAQ

**Q: How do I calculate the Bond Work Index?**
You can use the `calculate_bond_work_index` tool by providing the 80% passing size of the feed, the 80% passing size of the product, and the energy consumed during the test.

**Q: Can I account for dry grinding conditions?**
Yes, the `estimate_grinding_energy` tool includes a parameter to specify if the process is dry grinding, which applies the necessary adjustment factor.

**Q: How is circuit power determined?**
Use the `project_circuit_power` tool. It multiplies the specific energy requirement by the mass throughput to find the required power in kW or MW.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bond-work-index-calculator](https://vinkius.com/en/ai-agent-connect/bond-work-index-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bond Work Index Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bond-work-index-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bond Work Index Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bond-work-index-calculator": {
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
