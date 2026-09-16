# Asphaltene Deposition Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/asphaltene-deposition-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [simulation](../categories/simulation.md)

Predicts asphaltene precipitation and deposition in reservoirs and wellbores.

## Description
This MCP server provides advanced thermodynamic modeling to predict asphaltene instability. It allows AI agents to `analyze_stability_profile` for specific fluid compositions, `map_deposition_zones` along pressure and temperature paths, `calculate_deposition_rate` based on flow conditions, and `suggest_mitigation_plan` to manage deposition risks in oil production environments.


## Available Tools (4)
- **analyze_stability_profile**: Determine if a specific fluid composition is stable under given pressure and temperature conditions
- **calculate_deposition_rate**: Estimate the speed at which asphaltene solids accumulate on surfaces
- **map_deposition_zones**: Identify the physical or operational locations where asphaltene precipitation is likely to occur
- **suggest_mitigation_plan**: Provide actionable strategies to prevent or remediate deposition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Asphaltene Deposition Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is this oil composition stable at 3000 psi and 150 degrees Fahrenheit?"

**🤖 AI Agent:**
> The fluid is stable with a stability margin of 450 psi.

---

**👤 You:**
> "Where is the deposition risk highest along this pressure path?"

**🤖 AI Agent:**
> The highest risk zone is located at a depth of 5000 feet where pressure drops below 2500 psi.

---

**👤 You:**
> "What is the expected deposition rate for a steel pipe at this flow velocity?"

**🤖 AI Agent:**
> The predicted mass accumulation rate is 0.05 kg/m² per day.


## ❓ FAQ

**Q: How does the model determine deposition risk?**
The model uses `map_deposition_zones` to evaluate how pressure and temperature changes move the fluid through the asphaltene instability zone.

**Q: Can I get mitigation strategies?**
Yes, the `suggest_mitigation_plan` tool provides actionable strategies based on current risk levels and operational constraints.

**Q: What inputs are required for stability analysis?**
To use `analyze_stability_profile`, you must provide the oil composition, current system pressure, and current system temperature.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/asphaltene-deposition-model](https://vinkius.com/en/ai-agent-connect/asphaltene-deposition-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Asphaltene Deposition Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `asphaltene-deposition-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Asphaltene Deposition Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "asphaltene-deposition-model": {
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
