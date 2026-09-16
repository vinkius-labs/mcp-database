# Cyclic Steam Stimulation (CSS) Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cyclic-steam-stimulation-css-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design and optimize thermal EOR operations for heavy oil reservoirs.

## Description
This MCP server provides specialized tools for planning Cyclic Steam Stimulation (CSS) operations. It allows engineers to calculate necessary steam volumes using `plan_steam_injection`, determine optimal soak periods with `calculate_soak_duration`, and predict production outcomes via `estimate_recovery_cycle`. Additionally, you can monitor reservoir health using `evaluate_cycle_efficiency` to track how heat utilization and recovery change over multiple cycles.


## Available Tools (4)
- **calculate_soak_duration**: Finds the optimal time to let the well sit idle to maximize heat transfer
- **estimate_recovery_cycle**: Predicts the amount of oil produced and the total length of the cycle
- **evaluate_cycle_efficiency**: Assesses the health of the well by comparing current performance against theoretical maximums
- **plan_steam_injection**: Determines the necessary steam volume required to achieve thermal targets in a specific reservoir


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cyclic Steam Stimulation (CSS) Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the steam injection volume needed for a reservoir with 25% porosity, 150 mD permeability, an initial viscosity of 5000 cP, and a target viscosity of 50 cP."

**🤖 AI Agent:**
> The required steam injection volume is 4500 m3 with an estimated heat loss of 120 m3.

---

**👤 You:**
> "What is the optimal soak time for an injection volume of 3000 m3 in a reservoir with 100 mD permeability and a thermal diffusivity of 0.05?"

**🤖 AI Agent:**
> The optimal soak time is 12 days.

---

**👤 You:**
> "Estimate the recovery for the 2nd cycle where 4000 m3 of steam was injected, the soak time was 10 days, and porosity is 20%."

**🤖 AI Agent:**
> The expected oil recovery is 850 m3 and the total cycle duration is 25 days.


## ❓ FAQ

**Q: How do I plan a new steam injection phase?**
Use the `plan_steam_injection` tool by providing the reservoir porosity, permeability, and the target and initial oil viscosity levels.

**Q: Can I predict oil recovery for future cycles?**
Yes, the `estimate_recovery_cycle` tool predicts the expected oil recovery and total cycle duration based on your injection volume and soak time.

**Q: How is efficiency tracked over time?**
You can use `evaluate_cycle_efficiency` to compare the expected oil recovery against the steam volume injected, which accounts for the decline in efficiency as cycle numbers increase.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cyclic-steam-stimulation-css-designer](https://vinkius.com/en/ai-agent-connect/cyclic-steam-stimulation-css-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cyclic Steam Stimulation (CSS) Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cyclic-steam-stimulation-css-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cyclic Steam Stimulation (CSS) Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cyclic-steam-stimulation-css-designer": {
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
