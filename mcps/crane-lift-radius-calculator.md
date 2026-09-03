# Crane Lift Radius Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/crane-lift-radius-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate crane lift capacity, safety margins, and required counterweights.

## Description
This MCP server provides specialized engineering tools for crane operations. It allows AI agents to determine if a specific load can be safely lifted using `analyze_lift_capacity`, calculate the necessary mass for stability with `calculate_required_counterweight`, and adjust capacity based on environmental factors like wind and ground stability using `evaluate_environmental_impact`. Finally, `verify_stability_compliance` ensures the entire lift plan meets safety standards.


## Available Tools (4)
- **calculate_required_counterweight**: Calculates the amount of counterweight needed to maintain stability for a specific lift
- **evaluate_environmental_impact**: Adjusts the allowable lifting capacity based on wind and ground conditions
- **verify_stability_compliance**: Checks the overall safety profile of a planned lift against regulatory and manufacturer constraints
- **analyze_lift_capacity**: Determines if a specific load can be safely lifted at a given radius


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crane Lift Radius Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can a crane with model ID 'heavy-lift-01' safely lift 15 tonnes at a 10m radius with a 1.5t rigging weight?"

**🤖 AI Agent:**
> Yes, the maximum capacity at a 10m radius for this model is 22 tonnes, providing a safe margin for the 16.5 tonne total weight.

---

**👤 You:**
> "How much counterweight is needed for a 20 tonne load at 15m radius for model 'crane-x'?"

**🤖 AI Agent:**
> The required counterweight for this lift is 45 tonnes to maintain the necessary stability ratio.

---

**👤 You:**
> "What happens to my lifting capacity if the wind speed is 45 km/h and the ground is soft?"

**🤖 AI Agent:**
> The capacity is significantly reduced. The wind speed causes an exponential drop in capacity, and the soft ground condition applies an additional 0.5 multiplier to the allowable weight.


## ❓ FAQ

**Q: How does the tool account for wind speed?**
The `evaluate_environmental_impact` tool reduces the allowable lifting capacity based on wind speed, as higher speeds increase lateral forces and reduce stability.

**Q: Can I calculate the counterweight needed for a specific load?**
Yes, you can use `calculate_required_counterweight` to determine the exact mass needed to maintain stability for a given radius and load weight.

**Q: What factors affect the safety margin?**
The safety margin is determined by the difference between the maximum capacity (from `analyze_lift_capacity`) and the total weight, which includes both the load and the rigging weight.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/crane-lift-radius-calculator](https://vinkius.com/ai-agent-connect/crane-lift-radius-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crane Lift Radius Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crane-lift-radius-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crane Lift Radius Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crane-lift-radius-calculator": {
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
