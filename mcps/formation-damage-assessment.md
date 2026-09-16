# Formation Damage Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/formation-damage-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Analyze wellbore damage, skin factors, and permeability reduction.

## Description
This MCP server provides specialized tools for reservoir engineering to assess formation damage. Use `analyze_skin_factor` to determine the extent of wellbore damage from pressure and flow data. Evaluate chemical risks with `evaluate_fluid_compatibility` to predict damage from filtrate invasion. Quantify physical blockage using `quantify_permeability_loss` and forecast productivity improvements with `estimate_stimulation_gain` after remedial treatments.


## Available Tools (4)
- **analyze_skin_factor**: Determines the extent of wellbore damage using pressure and flow data
- **estimate_stimulation_gain**: Forecasts the productivity increase expected from remedial well treatments
- **evaluate_fluid_compatibility**: Predicts the likelihood and severity of damage caused by chemical interactions
- **quantify_permeability_loss**: Calculates the impact of physical blockage on reservoir flow capacity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Formation Damage Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the skin factor for a well with 100 mD permeability, 5m wellbore radius, and this well test data: {"pressureDrawdown": 50, "flowingRate": 200, "reservoirPressure": 3000}"

**🤖 AI Agent:**
> The calculated skin factor is 2.5 and the damage radius is 1.2 meters.

---

**👤 You:**
> "What is the expected productivity increase if I reduce the skin from 5 to 0 with a current flow rate of 500 bpd?"

**🤖 AI Agent:**
> The expected flow rate after stimulation is 1250 bpd, representing a 150% productivity improvement.

---

**👤 You:**
> "How much permeability is lost if the initial permeability is 200 mD, invasion depth is 2m, and fines migration factor is 0.5?"

**🤖 AI Agent:**
> The permeability reduction ratio is 0.4, resulting in an impaired zone permeability of 80 mD.


## ❓ FAQ

**Q: How do I calculate the skin factor?**
You can use the `analyze_skin_factor` tool by providing well test data, original permeability, and the wellbore radius.

**Q: Can I predict damage from drilling fluids?**
Yes, the `evaluate_fluid_compatibility` tool predicts damage likelihood by comparing rock mineralogy with fluid chemical compositions.

**Q: How much will stimulation improve my well?**
The `estimate_stimulation_gain` tool forecasts the expected flow rate and percentage improvement based on current and target skin factors.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/formation-damage-assessment](https://vinkius.com/en/ai-agent-connect/formation-damage-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Formation Damage Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `formation-damage-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Formation Damage Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "formation-damage-assessment": {
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
