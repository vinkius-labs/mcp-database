# Subsidence Prediction Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/subsidence-prediction-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environmental](../categories/environmental.md)

Predict surface subsidence and geological risks from reservoir compaction.

## Description
This MCP server provides specialized tools for geological engineering to model surface movement caused by subsurface reservoir compaction. Use `calculate_subsidence_profile` to determine the spatial distribution of vertical displacement, and `estimate_affected_area` to define the geographic footprint of the subsidence event. The model also includes `evaluate_fault_risk` to assess the likelihood of geological instability and `get_reservoir_summary` for high-level compaction analysis.


## Available Tools (4)
- **calculate_subsidence_profile**: Determine the spatial distribution and peak magnitude of surface movement
- **estimate_affected_area**: Define the geographic footprint of the subsidence event
- **evaluate_fault_risk**: Assess the likelihood of geological instability caused by predicted subsidence
- **get_reservoir_summary**: Provide a high-level overview of reservoir characteristics and impact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Subsidence Prediction Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the subsidence profile for a reservoir at 1500m depth, 50m thick, with 5m compaction and 200MPa overburden stiffness using the geertsma model."

**🤖 AI Agent:**
> The peak vertical displacement is 12.4 meters, with the subsidence profile tapering off as distance from the center increases.

---

**👤 You:**
> "What is the risk to a fault located 200m from a subsidence center with a max subsidence of 15m and a fault orientation of 45 degrees?"

**🤖 AI Agent:**
> The risk level is classified as high due to the proximity of the fault to the peak displacement.

---

**👤 You:**
> "Provide a summary for a reservoir at 2000m depth, 80m thick, with 10m compaction."

**🤖 AI Agent:**
> The compaction ratio is 0.125 and the pressure impact factor is 0.85.


## ❓ FAQ

**Q: How do I calculate the area affected by ground movement?**
You can use the `estimate_affected_area` tool by providing the subsidence profile data and a displacement threshold value.

**Q: Can this model predict fault reactivation?**
Yes, the `evaluate_fault_risk` tool assesses the likelihood of geological instability based on peak subsidence and proximity to known faults.

**Q: What models are supported for subsidence calculation?**
The `calculate_subsidence_profile` tool supports both Geertsma and numerical modeling approaches.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/subsidence-prediction-model](https://vinkius.com/en/ai-agent-connect/subsidence-prediction-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Subsidence Prediction Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `subsidence-prediction-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Subsidence Prediction Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "subsidence-prediction-model": {
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
