# Terminal Spill Response Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/terminal-spill-response-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [maritime](../categories/maritime.md)

Develop oil spill response plans by modeling discharge scenarios, environmental risk, and resource deployment.

## Description
This MCP server provides critical tools for maritime terminal safety and environmental protection. It allows AI agents to model oil spill scenarios by calculating the `get_worst_case_discharge` for specific terminal configurations. Users can predict oil movement using `simulate_oil_trajectory` based on wind and current data, identify ecological risks with `assess_area_sensitivity`, and evaluate resource sufficiency through `calculate_response_gap`. This enables rapid, data-driven decision-making during environmental emergencies.


## Available Tools (4)
- **get_worst_case_discharge**: Determines the maximum potential oil volume for a specific terminal configuration
- **assess_area_sensitivity**: Identifies and ranks the risks to specific environmental or economic zones
- **calculate_response_gap**: Evaluates if currently available resources are sufficient to contain the predicted spill
- **simulate_oil_trajectory**: Predicts the movement and spread of a spill based on environmental conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Terminal Spill Response Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the worst-case discharge for terminal T-402 if there is a tank rupture?"

**🤖 AI Agent:**
> The worst-case discharge for terminal T-402 during a tank rupture is 5,000 cubic meters with a discharge rate of 250 cubic meters per hour.

---

**👤 You:**
> "Predict the oil trajectory for a 500 cubic meter spill at lat 25.0, lng -80.0 with 10 knot wind and 2 knot current."

**🤖 AI Agent:**
> The oil is predicted to move North-East, covering a spread area of 1.2 square kilometers, with an arrival at the Coral Reef Sanctuary in 4.5 hours.

---

**👤 You:**
> "Are my resources sufficient for a spill covering 5000 square meters if I have 1000 meters of boom and 50 cubic meters per hour skimming capacity?"

**🤖 AI Agent:**
> No, the resources are insufficient. There is a boom deficit of 250 meters and a critical shortfall in skimming capacity.


## ❓ FAQ

**Q: How do I calculate the maximum potential oil release?**
You can use the `get_worst_case_discharge` tool by providing the terminal ID and the type of failure being simulated.

**Q: Can I predict where the oil will spread?**
Yes, the `simulate_oil_trajectory` tool predicts the movement and spread based on spill location, volume, wind, and water currents.

**Q: How do I know if my response equipment is enough?**
Use the `calculate_response_gap` tool to compare your available boom length and skimmer capacity against the predicted spill area and duration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/terminal-spill-response-plan](https://vinkius.com/en/ai-agent-connect/terminal-spill-response-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Terminal Spill Response Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `terminal-spill-response-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Terminal Spill Response Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "terminal-spill-response-plan": {
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
