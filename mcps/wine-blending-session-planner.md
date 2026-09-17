# Wine Blending Session Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-blending-session-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Optimizes wine blending trials and sensory evaluation logistics.

## Description
This MCP server provides a strategic planning engine for wine blending. It allows AI agents to calculate optimal trial formulations using `get_trial_formulations`, determine necessary component volumes with `calculate_component_requirements`, evaluate past blending trends via `analyze_blend_history`, and organize tasting sessions through `prepare_sensory_logistics`.


## Available Tools (4)
- **analyze_blend_history**: Evaluates previous blending results to inform future trial selection and identify trends
- **calculate_component_requirements**: Determines the total volume of each component wine needed to execute a planned series of trials
- **get_trial_formulations**: Generates a list of potential blend formulations that satisfy target specifications while optimizing for trial efficiency
- **prepare_sensory_logistics**: Organizes the physical tasting requirements for a session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Blending Session Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a list of blend formulations for Cabernet Sauvignon and Merlot to hit a specific target profile."

**🤖 AI Agent:**
> I have generated three trial formulations that optimize for maximum coverage of your target profile using the available Cabernet Sauvignon and Merlot components.

---

**👤 You:**
> "How much Merlot do I need for 10 tasters for the planned trials?"

**🤖 AI Agent:**
> Based on the trial plan and a taster count of 10, you will need 4.5 liters of Merlot in total.

---

**👤 You:**
> "What was the convergence rate for the last blending project?"

**🤖 AI Agent:**
> The convergence rate for the last project was 0.85, indicating a rapid movement toward the target specifications.


## ❓ FAQ

**Q: How does the tool optimize blending trials?**
The `get_trial_formulations` tool uses mathematical models to select a subset of formulations that maximizes coverage of the target blend space, minimizing the total number of tastings required.

**Q: Can I calculate the volume of wine needed for a tasting?**
Yes, you can use `calculate_component_requirements` to determine the total volume of each component wine needed for a specific trial plan, including a batch size multiplier.

**Q: How is palate fatigue managed during sessions?**
The `prepare_sensory_logistics` tool organizes the tasting order to mitigate palate fatigue, typically by sequencing lighter profiles before heavier ones.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-blending-session-planner](https://vinkius.com/en/ai-agent-connect/wine-blending-session-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Blending Session Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-blending-session-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Blending Session Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-blending-session-planner": {
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
