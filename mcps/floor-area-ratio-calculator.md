# Floor Area Ratio Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/floor-area-ratio-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Calculate maximum buildable footprint, total floor area, and green space compliance for any plot size in seconds.

## Description
## Building Development Feasibility Analysis

The process of developing a property is complex. It requires coordinating multiple, often conflicting, zoning constraints--from how much ground area you can cover (Site Coverage) to the total bulk allowed over all floors (FAR), and ensuring enough space for water absorption (Permeability).

**The Problem:** Traditional planning assessments are manual, slow, and require an expert to track these three distinct metrics simultaneously. A developer might calculate a high FAR but fail because they neglected minimum permeable area requirements, or vice versa.

**The Mechanism:** This MCP connects your AI agent directly to the core formulas of urban planning law. It uses three specialized functions to assess viability: 

1.  `max_site_coverage`: Determines the maximum *ground footprint* allowed by zoning occupancy limits for a given plot size.
2.  `max_total_area`: Calculates the total permitted floor area (FAR) across all stories, ensuring overall density compliance.
3.  `calculate_permeability`: Verifies that enough open, non-impervious space remains after accounting for building foundations and meeting minimum green space mandates.

By chaining these tools, your agent can perform a complete, multi-faceted feasibility check in one workflow, identifying the most restrictive constraint immediately.

**The Advantage:** You get instant, quantitative compliance checks against complex municipal codes. This moves development planning from guesswork to guaranteed calculation support.


## Available Tools
- **max_site_coverage**: Takes plot area and maximum site coverage percentage as inputs.

Calculate the maximum allowable ground footprint area for building construction based on site coverage limits
- **max_total_area**: Takes plot area, FAR percentage, and optionally a site coverage footprint area.

Calculate the maximum total floor area allowed on a plot based on Floor Area Ratio restrictions
- **calculate_permeability**: Takes lot area, minimum permeability percentage, and optionally a building footprint area.

Calculate minimum permeable area required and available buildable ground after accounting for green space requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Floor Area Ratio Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We have a plot of 10,000 sq units. The zoning requires a max site coverage of 60% and a minimum permeability of 30%. What is the maximum total floor area we can build?"

**🤖 AI Agent:**
> First, calculate the max footprint using `max_site_coverage(plotArea=10000, maxSiteCoveragePercentage=0.6)`. Next, use that result and run `calculate_permeability(lotArea=10000, minPermeabilityPercentage=0.3, grossBuildingFootprintArea=<result from previous step>)` to find the actual usable footprint. Finally, input this reduced footprint into `max_total_area(plotArea=10000, maxFARPercentage=2.5, siteCoverageFootprintArea=<usable footprint>)` for the final answer.

---

**👤 You:**
> "Given a 100 sq unit plot with an FAR of 2.5, what is our maximum total buildable area?"

**🤖 AI Agent:**
> Run the `max_total_area` tool: `max_total_area(plotArea=100, maxFARPercentage=2.5, siteCoverageFootprintArea=null)`. This will give you a quick estimate of total density compliance.

---

**👤 You:**
> "Verify that our proposed 40% ground footprint on a 5,000 sq unit lot meets zoning standards for occupancy."

**🤖 AI Agent:**
> Use the `max_site_coverage` tool: `max_site_coverage(plotArea=5000, maxSiteCoveragePercentage=0.4)`. This will confirm if your proposed footprint is within the legal limit set by the zoning code.


## ❓ FAQ

**Q: If I increase the building size, which constraint is most likely to fail first: Site Coverage or Permeability?**
The relationship between these constraints is complex. You must run `max_site_coverage` first to find the maximum ground footprint. Then, use this result in `calculate_permeability`. The permeability check will often be the most restrictive physical constraint because it mandates a minimum unpaved area before considering building size.

**Q: Can I calculate the total buildable space without knowing the ground footprint?**
Yes, you can use `max_total_area` with just the plot area and the FAR ratio. However, for a complete assessment, you should always run `calculate_permeability` as well, because permeability might force your buildable footprint to be smaller than what `max_total_area` assumes.

**Q: What is the role of plotArea in these calculations?**
The `plotArea` (or `lotArea`) is your fixed starting point--the total surface area of the land parcel. It serves as the base input for all three tools (`max_site_coverage`, `max_total_area`, and `calculate_permeability`), providing the dimensional context against which zoning rules are applied.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/floor-area-ratio-calculator](https://vinkius.com/mcp/floor-area-ratio-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Floor Area Ratio Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `floor-area-ratio-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Floor Area Ratio Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "floor-area-ratio-calculator": {
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
