# Production Logging Interpretation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/production-logging-interpretation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Analyze PLT data to identify fluid entry points and production profiles.

## Description
This MCP server provides specialized tools for interpreting Production Logging Tool (PLT) data. It allows AI agents to analyze spinner, temperature, pressure, and holdup measurements to determine zonal contributions, locate fluid entry points, and characterize flow regimes. By accounting for multiphase flow and wellbore deviation, it provides a precise view of wellbore production behavior.


## Available Tools (4)
- **analyze_flow_regime**: Determines the physical flow pattern (e.g., mist, slug, bubble) at specific depths
- **calculate_zonal_contributions**: Determines how much each individual formation zone is contributing to the total fluid production
- **get_production_profile**: Provides a complete summary of the production behavior across the entire wellbore depth
- **identify_entry_points**: Locates specific depths where fluids are entering the wellbore from the formation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Production Logging Interpretation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the production profile for a wellbore with a depth of 5000m and an inclination of 30 degrees?"

**🤖 AI Agent:**
> The production profile shows a total flow rate of 1250 bbl/d with a slug flow regime at 2500m and an annular regime at 4500m.

---

**👤 You:**
> "Identify the entry points using this temperature data: [{'depth': 1000, 'temp': 80}, {'depth': 1001, 'temp': 75}] and pressure data: [{'depth': 1000, 'pressure': 2000}, {'depth': 1001, 'pressure': 1950}]."

**🤖 AI Agent:**
> A fluid entry point was detected at 1001m with a high entry intensity, likely indicating gas influx.

---

**👤 You:**
> "Calculate the zonal contributions for these zones: [{'topDepth': 1000, 'bottomDepth': 2000, 'zoneName': 'Zone A'}, {'topDepth': 2000, 'bottomDepth': 3000, 'zoneName': 'Zone B'}]."

**🤖 AI Agent:**
> Zone A contributes 65% of the total flow, while Zone B contributes 35%.


## ❓ FAQ

**Q: How can I find where fluids are entering the wellbore?**
You can use the `identify_entry_points` tool by providing temperature and pressure data arrays.

**Q: Can this tool calculate how much each zone is producing?**
Yes, the `calculate_zonal_contributions` tool determines the fluid rate and percentage contribution for each defined zone.

**Q: Does the analysis account for wellbore inclination?**
Yes, tools like `get_production_profile` and `analyze_flow_regime` require inclination to account for gravity-driven segregation and flow patterns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/production-logging-interpretation](https://vinkius.com/en/ai-agent-connect/production-logging-interpretation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Production Logging Interpretation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `production-logging-interpretation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Production Logging Interpretation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "production-logging-interpretation": {
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
