# Site Remediation Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/site-remediation-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Generates comprehensive remediation strategies, timelines, and cost estimates for contaminated sites.

## Description
This MCP server provides professional decision-support for environmental engineers and site managers. It connects AI agents to specialized remediation logic to calculate optimal cleanup strategies. Using `plan_remediation`, agents can generate full strategies including technology selection, estimated duration, and cost projections. The server also provides granular tools like `evaluate_feasibility` to test specific technologies against site conditions, `calculate_timeline` for duration modeling, and `estimate_remediation_cost` for financial forecasting based on volume and approach type.


## Available Tools (4)
- **calculate_timeline**: Calculates the expected time required to reach cleanup goals
- **estimate_remediation_cost**: Provides a financial projection for the proposed remediation work
- **evaluate_feasibility**: Determines if a specific remediation technology is suitable for the site
- **plan_remediation**: Generates a full remediation strategy including technology selection, timeline, and cost


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Site Remediation Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a remediation plan for a site with Lead concentrations at 500mg/kg and a cleanup goal of 100mg/kg. Soil permeability is low and groundwater is at 5 meters."

**🤖 AI Agent:**
> The recommended approach is active remediation using soil excavation and stabilization. The estimated duration is 14 months with a projected cost of $450,000.

---

**👤 You:**
> "Is thermal desorption feasible for a site contaminated with Heavy Metals and low soil permeability?"

**🤖 AI Agent:**
> No, thermal desorption is not feasible for this site because heavy metals are non-volatile and require physical removal or stabilization instead.

---

**👤 You:**
> "Estimate the cost for an active remediation approach treating 5000 cubic meters of soil using soil excavation."

**🤖 AI Agent:**
> The estimated total cost for treating 5000 cubic meters via soil excavation is $320,000, including mobilization and energy expenses.


## ❓ FAQ

**Q: How does the tool decide between active and passive remediation?**
The decision is driven by the gap between current contaminant concentrations and cleanup goals, as well as site-specific factors like `soilPermeability`. If the gap is extreme or permeability is too low for natural movement, the engine prioritizes active remediation.

**Q: Can I check if a specific technology is suitable for my site?**
Yes, you can use the `evaluate_feasibility` tool to determine if a specific technology is physically and chemically suitable based on your site's contaminants and physical parameters.

**Q: What inputs are required for a full remediation plan?**
To use `plan_remediation`, you must provide the list of contaminant types, their current concentrations, the target cleanup goals, and site conditions such as soil permeability and groundwater depth.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/site-remediation-planner](https://vinkius.com/ai-agent-connect/site-remediation-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Site Remediation Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `site-remediation-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Site Remediation Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "site-remediation-planner": {
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
