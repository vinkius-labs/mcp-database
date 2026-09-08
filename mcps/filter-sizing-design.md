# Filter Sizing Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/filter-sizing-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Technical sizing for dewatering equipment based on slurry characteristics.

## Description
This MCP server provides specialized engineering tools for dewatering equipment design. It allows AI agents to calculate critical parameters such as filter area, cycle time, and filtration rate by analyzing slurry solids concentration, target moisture, and throughput. Users can utilize `query_filter_sizing` to determine design requirements, `validate_feed_suitability` to assess feasibility, `compare_filtration_modes` to evaluate vacuum versus pressure filtration, and `estimate_cake_resistance` to model cake permeability.


## Available Tools (4)
- **compare_filtration_modes**: Compares the required filter area and expected cycle times between vacuum and pressure filtration for the same feed
- **estimate_cake_resistance**: Calculates the resistance offered by the filter cake based on particle characteristics
- **query_filter_sizing**: Calculates the primary design parameters (Area, Cycle Time, Rate) for a specific dewatering scenario
- **validate_feed_suitability**: Determines if a specific slurry can realistically be dewatered to a target moisture level using the chosen method


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Filter Sizing Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the filter area needed for a slurry with 30% solids, 15% target moisture, and 50 m3/h throughput using vacuum filtration."

**🤖 AI Agent:**
> The required filter area for this vacuum filtration scenario is 125 m2 with a cycle time of 45 minutes.

---

**👤 You:**
> "Is it feasible to reach 10% moisture using vacuum filtration for a slurry with 25% solids concentration?"

**🤖 AI Agent:**
> No, vacuum filtration is not feasible for this target; the risk level is high due to the low moisture requirement.

---

**👤 You:**
> "Compare vacuum and pressure filtration for 40% solids and 12% target moisture at 100 m3/h throughput."

**🤖 AI Agent:**
> Pressure filtration requires 45 m2 of area, whereas vacuum filtration requires 180 m2, providing an area reduction factor of 4.0.


## ❓ FAQ

**Q: How do I calculate the required filter area?**
You can use the `query_filter_sizing` tool by providing the slurry solids concentration, target moisture, required throughput, and the filtration type.

**Q: Can I compare vacuum and pressure filtration?**
Yes, the `compare_filtration_modes` tool provides a direct comparison of required area and cycle times between vacuum and pressure methods.

**Q: How is cake resistance determined?**
The `estimate_cake_resistance` tool calculates specific cake resistance and permeability based on particle size and solids concentration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/filter-sizing-design](https://vinkius.com/ai-agent-connect/filter-sizing-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Filter Sizing Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `filter-sizing-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Filter Sizing Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "filter-sizing-design": {
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
