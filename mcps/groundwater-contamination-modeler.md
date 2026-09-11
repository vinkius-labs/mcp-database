# Groundwater Contamination Modeler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/groundwater-contamination-modeler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environmental-science](../categories/environmental-science.md)

Predicts hydrocarbon plume migration, contaminant concentrations, and remediation needs.

## Description
This MCP server provides specialized tools for modeling the environmental impact of hydrocarbon releases in groundwater systems. It allows AI agents to predict the spatial movement of contaminant plumes using `get_plume_migration_path`, calculate concentration profiles over time with `calculate_concentration_profile`, assess necessary cleanup efforts via `assess_remediation_needs`, and evaluate soil containment capabilities through `simulate_soil_impact`.


## Available Tools (4)
- **assess_remediation_needs**: Identifies the necessary actions and estimated scale of cleanup required to meet safety standards
- **calculate_concentration_profile**: Determines the concentration of the contaminant at specific points and time intervals
- **get_plume_migration_path**: Predicts the spatial movement and direction of the contaminant plume from the release site
- **simulate_soil_impact**: Evaluates how soil properties influence the containment of the release


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Groundwater Contamination Modeler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the movement of a 500L hydrocarbon release in soil with 0.3 permeability and 0.5 groundwater velocity at 10m depth."

**🤖 AI Agent:**
> The contaminant plume is expected to move in the direction of the hydraulic gradient with an estimated travel distance of 150 meters and a plume radius of 45 meters.

---

**👤 You:**
> "What will the concentration be for a 1000L release after 30 days, given an adsorption coefficient of 0.2 and biodegradation rate of 0.05?"

**🤖 AI Agent:**
> The current concentration after 30 days is 12.5 mg/L, with a peak concentration of 45.0 mg/L recorded earlier.

---

**👤 You:**
> "Determine the cleanup needed for a concentration of 50 mg/L when the target is 5 mg/L in a 1000m3 aquifer."

**🤖 AI Agent:**
> The required remediation type is pump-and-treat, with an estimated cleanup volume of 850m3 and a duration of 12 months.


## ❓ FAQ

**Q: How does the model account for natural cleanup?**
The model uses `calculate_concentration_profile` to factor in biodegradation rates, which represents the natural breakdown of contaminants by microorganisms.

**Q: Can I predict where the contamination will spread?**
Yes, by using the `get_plume_migration_path` tool, you can estimate the direction and distance the contaminant plume will travel based on soil permeability and groundwater velocity.

**Q: What information is needed to assess remediation?**
To use `assess_remediation_needs`, you must provide the current contaminant concentration, the target safety concentration, and the total volume of the affected aquifer.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/groundwater-contamination-modeler](https://vinkius.com/en/ai-agent-connect/groundwater-contamination-modeler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Groundwater Contamination Modeler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `groundwater-contamination-modeler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Groundwater Contamination Modeler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "groundwater-contamination-modeler": {
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
