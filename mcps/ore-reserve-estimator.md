# Ore Reserve Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ore-reserve-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analysis](../categories/data-analysis.md)

Estimates mineral ore reserves using geostatistical interpolation and geological constraints.

## Description
This MCP server provides specialized tools for mineral resource estimation. It allows AI agents to calculate ore tonnage and grade using methods like `calculate_tonnage_and_grade`, classify reserves into Proven or Probable via `classify_reserves`, and define spatial limits with `define_geological_domain`. It also includes `validate_data_integrity` to ensure drilling and assay data are consistent before processing.


## Available Tools (4)
- **calculate_tonnage_and_grade**: Determines the total mass and the average concentration of the target metal within a defined area
- **classify_reserves**: Assigns a confidence level (Proven or Probable) to the calculated reserves based on data density
- **define_geological_domain**: Sets the spatial boundaries within which ore estimation is allowed to occur
- **validate_data_integrity**: Ensures the provided drilling and assay data are spatially and logically consistent before processing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ore Reserve Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the tonnage and grade for these samples with a density of 2.7 and a cut-off grade of 0.5 using kriging."

**🤖 AI Agent:**
> The total tonnage is 1,250,000 tonnes with an average grade of 0.85% copper.

---

**👤 You:**
> "Classify the reserves with a continuity index of 0.8 and a sampling density threshold of 25."

**🤖 AI Agent:**
> The reserves are classified as 450,000 tonnes of Proven ore and 800,000 tonnes of Probable ore.

---

**👤 You:**
> "Check if my drilling data is consistent."

**🤖 AI Agent:**
> The data integrity check passed successfully with no errors found.


## ❓ FAQ

**Q: What interpolation methods are supported?**
The server supports Kriging and Inverse Distance Weighting (IDW) through the `calculate_tonnage_and_grade` tool.

**Q: How are reserves classified?**
Reserves are classified as Proven or Probable using the `classify_reserves` tool based on sampling density and geological continuity.

**Q: Can I define specific geological boundaries?**
Yes, you can use `define_geological_domain` to set spatial boundaries to prevent grade leakage into waste zones.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ore-reserve-estimator](https://vinkius.com/ai-agent-connect/ore-reserve-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ore Reserve Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ore-reserve-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ore Reserve Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ore-reserve-estimator": {
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
