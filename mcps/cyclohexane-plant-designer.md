# Cyclohexane Plant Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cyclohexane-plant-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Engineering tool for designing cyclohexane production plants via benzene hydrogenation.

## Description
This MCP server provides specialized engineering tools for designing industrial cyclohexane production plants. It allows users to calculate reactor dimensions using `calculate_reactor_spec`, determine hydrogen requirements with `estimate_hydrogen_demand`, validate product quality via `verify_purity_compliance`, and perform comparative analysis between liquid and vapor phases using `compare_phase_efficiency`.


## Available Tools (4)
- **calculate_reactor_spec**: Determines the necessary physical dimensions and operational parameters of the reactor
- **compare_phase_efficiency**: Provides a comparative analysis of liquid-phase vs. vapor-phase for a specific set of inputs
- **estimate_hydrogen_demand**: Calculates the total hydrogen required to support the planned production
- **verify_purity_compliance**: Validates if the designed process can meet the specific purity requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cyclohexane Plant Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the reactor specifications for a liquid-phase process with a benzene feed rate of 500, target capacity of 450, and purity threshold of 0.99."

**🤖 AI Agent:**
> The reactor requires a volume of 12.5 m³, a height of 4.2 m, an optimal temperature of 150°C, an optimal pressure of 25 bar, and 150 kg of catalyst mass.

---

**👤 You:**
> "How much hydrogen do I need for a vapor-phase process with 400 benzene feed and 95% conversion efficiency?"

**🤖 AI Agent:**
> The total hydrogen flow rate required is 125.5 kg/h, consisting of 114.0 kg/h stoichiometric hydrogen and 11.5 kg/h excess hydrogen.

---

**👤 You:**
> "Will my design meet a 99.5% purity requirement with a 15 m³ reactor at 160°C in the liquid phase?"

**🤖 AI Agent:**
> The predicted purity is 99.7%, which is compliant with your 99.5% threshold.


## ❓ FAQ

**Q: How do I design a reactor for my plant?**
You can use the `calculate_reactor_spec` tool by providing the benzene feed rate, target capacity, purity threshold, and the chosen process phase.

**Q: Can I compare liquid and vapor phase processes?**
Yes, the `compare_phase_efficiency` tool provides a comparative analysis of metrics and recommendations for both phases.

**Q: How is hydrogen consumption calculated?**
The `estimate_hydrogen_demand` tool calculates the total hydrogen flow rate required based on benzene feed, phase, and conversion efficiency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cyclohexane-plant-designer](https://vinkius.com/en/ai-agent-connect/cyclohexane-plant-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cyclohexane Plant Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cyclohexane-plant-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cyclohexane Plant Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cyclohexane-plant-designer": {
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
