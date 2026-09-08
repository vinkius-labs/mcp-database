# Kriging Estimation Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/kriging-estimation-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Perform Ordinary Kriging to estimate block grades and spatial uncertainty.

## Description
This MCP server provides geostatistical tools for resource modeling using Ordinary Kriging. It allows AI agents to calculate block grades, estimation variances, and kriging weights from spatial sample data. Users can validate variogram parameters with `validate_variogram_parameters`, analyze sample density via `get_spatial_correlation_stats`, and retrieve specific sample influences using `get_kriging_weights`. The engine supports anisotropy and search ellipse constraints for precise spatial interpolation.


## Available Tools (4)
- **get_block_estimates**: Calculates the estimated grade and uncertainty for a specific set of block discretization points
- **get_kriging_weights**: Retrieves the specific influence (weights) each sample has on a target estimation point
- **get_spatial_correlation_stats**: Provides high-level summary statistics regarding the density and distribution of samples within the search space
- **validate_variogram_parameters**: Ensures the variogram model provided is physically and mathematically sound for kriging


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kriging Estimation Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the estimated grade for these block points using the provided sample data and variogram."

**🤖 AI Agent:**
> The estimated grade for the target block is 4.52 g/t with an estimation variance of 0.12.

---

**👤 You:**
> "What are the weights for the samples near the center point (10, 10, 10)?"

**🤖 AI Agent:**
> The sample at (10, 10, 10) has a weight of 0.65, and the sample at (12, 10, 10) has a weight of 0.35.

---

**👤 You:**
> "Check the spatial correlation statistics for my sample data within a 50m radius."

**🤖 AI Agent:**
> Within the 50m search radius, there are 12 samples with an average distance to target of 24.5m and a coverage density of 0.08.


## ❓ FAQ

**Q: What is Ordinary Kriging?**
Ordinary Kriging is a geostatistical interpolation method that estimates values at unsampled locations by weighting nearby known samples based on spatial correlation.

**Q: How do I ensure my variogram model is valid?**
You can use the `validate_variogram_parameters` tool to check if your nugget, sill, and range parameters are mathematically sound.

**Q: Can this model handle directional dependencies?**
Yes, the model accounts for anisotropy and uses a search ellipse to define the spatial boundary for sample selection.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/kriging-estimation-model](https://vinkius.com/ai-agent-connect/kriging-estimation-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kriging Estimation Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kriging-estimation-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kriging Estimation Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kriging-estimation-model": {
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
