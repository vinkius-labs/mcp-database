# Tailings Storage Facility Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tailings-storage-facility-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design tailings storage facilities (TSFs) using production, topography, and water balance data.

## Description
This MCP server provides specialized engineering tools for designing tailings storage facilities (TSFs). It allows users to calculate storage capacity, determine embankment requirements for different construction methods, and simulate water balance. By integrating production rates and site topography, the tool can generate a complete design summary including estimated lifespan and stability status. Use `analyze_storage_capacity` to find available volume, `calculate_embankment_requirements` for dam wall specifications, `simulate_water_balance` for water level fluctuations, and `design_tsf_lifecycle` for a full design overview.


## Available Tools (4)
- **analyze_storage_capacity**: Determines the total volume available for tailings and water based on site layout
- **calculate_embankment_requirements**: Determines the necessary height and volume of the dam wall
- **design_tsf_lifecycle**: Generates a comprehensive design summary by integrating production, topography, and water management
- **simulate_water_balance**: Evaluates how water levels will fluctuate within the facility over time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tailings Storage Facility Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the storage capacity for a site with a total area of 500,000 m2 and an average depth of 20m, with a tailings density of 1.6."

**🤖 AI Agent:**
> The total storage capacity for the specified site is 10,000,000 m3.

---

**👤 You:**
> "What are the embankment requirements for a downstream construction with a target volume of 5,000,000 m3?"

**🤖 AI Agent:**
> The required embankment height is 45 meters with a wall volume of 2,250,000 m3.

---

**👤 You:**
> "Generate a full TSF design summary for a production rate of 2,000,000 m3/year using centerline construction."

**🤖 AI Agent:**
> The design summary shows a total capacity of 10,000,000 m3, an embankment height of 40 meters, and an estimated lifespan of 5 years.


## ❓ FAQ

**Q: What construction methodologies are supported?**
The tool supports upstream, downstream, and centerline construction methodologies for embankment design.

**Q: How is the facility lifespan calculated?**
The estimated lifespan is calculated by dividing the total storage capacity by the tailings production rate.

**Q: Can I simulate water fluctuations?**
Yes, you can use the `simulate_water_balance` tool to evaluate how precipitation, evaporation, and seepage affect water levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tailings-storage-facility-design](https://vinkius.com/en/ai-agent-connect/tailings-storage-facility-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tailings Storage Facility Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tailings-storage-facility-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tailings Storage Facility Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tailings-storage-facility-design": {
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
