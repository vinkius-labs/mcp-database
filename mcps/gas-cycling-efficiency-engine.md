# Gas Cycling Efficiency Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/gas-cycling-efficiency-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate sweep efficiency, gas dilution, and condensate recovery in reservoirs.

## Description
This MCP server provides specialized calculation tools for evaluating gas cycling performance in condensate reservoirs. It allows AI agents to determine how effectively injected gas displaces hydrocarbons by calculating `calculate_sweep_efficiency` to assess reservoir contact, `calculate_dry_gas_dilution` to measure fluid composition changes, and `calculate_recovery_factor` to quantify total condensate yield. The engine also provides `evaluate_cycling_performance` for a comprehensive operational overview.


## Available Tools (4)
- **calculate_dry_gas_dilution**: Measures the impact of injected gas on the composition of the produced fluids
- **calculate_recovery_factor**: Quantifies the total amount of condensate successfully recovered through the cycling process
- **calculate_sweep_efficiency**: Determines how effectively the injected gas is contacting the reservoir volume
- **evaluate_cycling_performance**: Provides a high-level summary of the entire gas cycling operation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gas Cycling Efficiency Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected recovery factor for 1,000,000 units of condensate with a sweep efficiency of 0.7 and a dilution factor of 0.8?"

**🤖 AI Agent:**
> The total volume recovered is 560,000 units, resulting in a recovery factor of 0.56.

---

**👤 You:**
> "Calculate the sweep efficiency for a reservoir with a heterogeneity factor of 0.3, an injection rate of 500, and a permeability map of {'zone1': 100, 'zone2': 150}."

**🤖 AI Agent:**
> The calculated sweep efficiency is 0.78 with a contact ratio of 0.82.

---

**👤 You:**
> "How much will the injected gas dilute the reservoir gas if the mixing ratio is 0.5 and the injected gas is 95% methane?"

**🤖 AI Agent:**
> The dilution factor is 0.45, resulting in a produced gas purity of 0.92.


## ❓ FAQ

**Q: How do I calculate the total condensate recovered?**
You can use the `calculate_recovery_factor` tool, providing the initial condensate in place, the sweep efficiency, and the dilution factor.

**Q: Can I get a full performance summary?**
Yes, the `evaluate_cycling_performance` tool aggregates injection, reservoir, and production data into a single performance score.

**Q: What factors affect sweep efficiency?**
Sweep efficiency is determined by the permeability map, injection rate, and the heterogeneity factor of the reservoir.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/gas-cycling-efficiency-engine](https://vinkius.com/en/ai-agent-connect/gas-cycling-efficiency-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gas Cycling Efficiency Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gas-cycling-efficiency-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gas Cycling Efficiency Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gas-cycling-efficiency-engine": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
