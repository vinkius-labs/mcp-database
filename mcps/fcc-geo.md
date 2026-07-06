# FCC Geo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fcc-geo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [telecommunications](../categories/telecommunications.md)

Instantly convert geographic coordinates into precise US Census Blocks and Telecommunication zones with zero authentication.

## Description
The **FCC Geo MCP Server** connects your AI agent directly to the United States Federal Communications Commission's geographic intelligence endpoints. Completely frictionless and requiring zero API keys, it provides instant spatial intersection analysis.

### Core Capabilities

- **Census Block Resolution** — Convert any latitude and longitude across the US into precise State, County, and Census Block FIPS codes.
- **Telecom Territorial Mapping** — Discover precisely which Cellular Market Areas (CMA), Economic Area Groupings (EAG), and spectrum licensing zones overlap with any physical location.
- **Zero-Friction Access** — Fully open and unmetered endpoints, removing all authentication barriers for immediate geospatial data engineering.

Ideal for real estate analysts, logistics AI systems, urban planners, and spectrum licensing researchers needing instantaneous conversion from coordinates to official US government zones.


## Available Tools (2)
- **get_fcc_areas_by_lat_lon**: Retrieve FCC telecommunication boundaries (CMA, PEA, EAG) intersecting given coordinates
- **get_census_block_by_lat_lon**: Essential for mapping physical spaces to regulatory regions.

Convert exact geographic coordinates into US Census Blocks, Counties, and FIPS codes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FCC Geo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the Census Block for coordinates 40.0 latitude and -85.0 longitude."

**🤖 AI Agent:**
> I've checked the FCC geodatabase. Those coordinates correspond to Wayne County in Indiana (State FIPS 18, County FIPS 18177). The exact Census Block FIPS code is 181770103002008.

---

**👤 You:**
> "Which telecommunication economic areas overlap with coordinates 40, -85?"

**🤖 AI Agent:**
> According to the FCC Area boundaries, coordinates 40.0, -85.0 fall under Cellular Market Area (CMA) 408, Major Economic Area (MEA) 019, and Economic Area Grouping (EAG) 704.

---

**👤 You:**
> "Convert the coordinate pair 34.05, -118.24 into proper Census details."

**🤖 AI Agent:**
> Checking the FCC Geo repository...
Coordinates map directly to California (State FIPS 06), Los Angeles County (County FIPS 06037). The block FIPS evaluates firmly to 060372074001004 natively effortlessly.


## ❓ FAQ

**Q: Do I need to pay or provide an API Key?**
Neither! The FCC Geo API operates completely publicly. There are zero auth steps, meaning you can plug it into any AI agent securely and immediately.

**Q: How accurate is the coordinate conversion?**
It draws directly from US federal census files. When you submit raw geographic decimal degrees, the system instantly identifies the overlapping demographic and telecommunication limits with absolute national accuracy.

**Q: Can I query locations outside of the United States?**
No. The FCC Geo API specifically maps United States territories and census blocks. International coordinates will not return valid census or telecommunication zone data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fcc-geo](https://vinkius.com/mcp/fcc-geo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FCC Geo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fcc-geo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FCC Geo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fcc-geo": {
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
