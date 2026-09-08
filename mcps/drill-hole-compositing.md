# Drill Hole Compositing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/drill-hole-compositing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-science](../categories/data-science.md)

Standardize irregular assay data into uniform intervals for geological modeling.

## Description
This MCP server provides specialized tools for transforming irregular drill hole assay measurements into standardized, equal-length intervals. It is essential for geological modeling and statistical analysis to prevent bias from varying sample lengths. Use `get_composites` to generate uniform intervals, `get_composite_statistics` for statistical summaries, `validate_interval_consistency` to check for depth overlaps, and `get_compositing_summary` to verify mass preservation.


## Available Tools (4)
- **get_composite_statistics**: Provides summary statistics for a set of generated composites
- **get_composites**: Generates a standardized sequence of composite intervals and grades from raw assay data
- **get_compositing_summary**: Provides a high-level comparison between raw assay data and the resulting composites
- **validate_interval_consistency**: Checks if the input assay data or composites contain overlapping or illogical depth ranges


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Drill Hole Compositing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate 2-meter composites from this assay data: [{'startDepth': 0, 'endDepth': 5, 'grade': 1.2}, {'startDepth': 5, 'endDepth': 10, 'grade': 0.8}]"

**🤖 AI Agent:**
> [{'startDepth': 0, 'endDepth': 2, 'grade': 1.2}, {'startDepth': 2, 'endDepth': 4, 'grade': 1.2}, {'startDepth': 4, 'endDepth': 6, 'grade': 1.0}, {'startDepth': 6, 'endDepth': 8, 'grade': 0.8}, {'startDepth': 8, 'endDepth': 10, 'grade': 0.8}]

---

**👤 You:**
> "What are the mean and max grades for these composites: [{'startDepth': 0, 'endDepth': 2, 'grade': 1.5}, {'startDepth': 2, 'endDepth': 4, 'grade': 2.5}]"

**🤖 AI Agent:**
> The mean grade is 2.0 and the maximum grade is 2.5.

---

**👤 You:**
> "Check if these intervals are valid: [{'startDepth': 10, 'endDepth': 5}]"

**🤖 AI Agent:**
> The intervals are invalid because the start depth is greater than the end depth.


## ❓ FAQ

**Q: How does the tool handle geological boundaries?**
You can provide `boundaryDepths` to the `get_composites` tool. This ensures that the compositing process resets at these specific depths, preventing the mixing of data across different geological units.

**Q: Can I check if my data has overlapping intervals?**
Yes, use the `validate_interval_consistency` tool to detect overlapping or out-of-order depth ranges in your assay data or composites.

**Q: How is mass preservation verified?**
The `get_compositing_summary` tool provides a `totalMassPreservationRatio`. A value of 1.0 indicates that the total metal mass was perfectly preserved during the transformation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/drill-hole-compositing](https://vinkius.com/ai-agent-connect/drill-hole-compositing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Drill Hole Compositing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `drill-hole-compositing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Drill Hole Compositing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "drill-hole-compositing": {
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
