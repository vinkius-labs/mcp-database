# Groundwater Monitoring Program Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/groundwater-monitoring-program-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [compliance](../categories/compliance.md)

Design comprehensive groundwater monitoring strategies including well placement and sampling schedules.

## Description
This MCP server provides specialized tools for designing groundwater monitoring programs. It integrates site hydrogeology, contaminant profiles, and regulatory constraints to determine optimal well placement, sampling frequency, and required analytical parameters. Use `design_well_network` to establish spatial distribution, `calculate_sampling_schedule` to set collection intervals, `generate_parameter_list` to identify necessary chemical tests, and `validate_compliance` to audit the final program against regulatory standards.


## Available Tools (4)
- **validate_compliance**: Audits a proposed monitoring program against specific regulatory and hydrogeological constraints
- **calculate_sampling_schedule**: Establishes how often water samples must be collected from the defined well network
- **design_well_network**: Determines the optimal spatial distribution and quantity of monitoring wells for a site
- **generate_parameter_list**: Defines the specific chemical or biological substances that must be tested for


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Groundwater Monitoring Program Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Design a well network for a site with a north-flowing gradient, a sandy aquifer, and a plume area of 50m width by 200m length."

**🤖 AI Agent:**
> The optimized network requires 6 wells: 1 upgradient well to establish baseline quality and 5 downgradient wells distributed along the leading edge of the plume to capture migration.

---

**👤 You:**
> "What parameters should I test for if I suspect benzene contamination under US-EPA-GW regulations?"

**🤖 AI Agent:**
> The required testing includes benzene, toluene, ethylbenzene, and xylenes (BTEX), along with mandatory baseline indicators such as pH, conductivity, and dissolved oxygen.

---

**👤 You:**
> "Is my monitoring program compliant if I only have one downgradient well for a high-risk site?"

**🤖 AI Agent:**
> No, the program is non-compliant. For a high-risk site, the `validate_compliance` check indicates that the downgradient well count is insufficient to capture the plume width.


## ❓ FAQ

**Q: How do I determine where to place monitoring wells?**
You can use the `design_well_network` tool. Provide the site hydrogeology (gradient, flow direction, aquifer type) and the estimated contaminant plume area to receive an optimized well count and location plan.

**Q: Can this tool help with regulatory compliance?**
Yes. The `validate_compliance` tool audits your proposed monitoring program against specific regulatory and hydrogeological constraints to identify any deficiencies.

**Q: How often should I sample my groundwater?**
The `calculate_sampling_schedule` tool determines the frequency based on your well network, the volatility of the contaminants, and the specific regulatory standard you are following.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/groundwater-monitoring-program-designer](https://vinkius.com/ai-agent-connect/groundwater-monitoring-program-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Groundwater Monitoring Program Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `groundwater-monitoring-program-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Groundwater Monitoring Program Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "groundwater-monitoring-program-designer": {
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
