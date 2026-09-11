# Intelligent Completion Design Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/intelligent-completion-design-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Design intelligent completion systems by calculating ICV sizes, control lines, and HPU requirements.

## Description
This engine automates the complex engineering required for intelligent completion design. It synthesizes reservoir requirements and zonal properties to determine optimal hardware configurations. Use `calculate_icv_sizing` to determine valve diameters and types, `estimate_control_lines` to calculate necessary conduits, `size_hpu` to determine surface power requirements, and `generate_monitoring_layout` to plan downhole sensor placement.


## Available Tools (4)
- **calculate_icv_sizing**: Determines the appropriate diameter and type for Intelligent Completion Valves (ICVs) to meet zonal flow demands
- **estimate_control_lines**: Calculates the quantity and type of control lines needed to connect surface equipment to downhole components
- **generate_monitoring_layout**: Designs the placement and configuration of downhole sensors to satisfy monitoring needs
- **size_hpu**: Sizes the surface Hydraulic Power Unit required to actuate all downhole components


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Intelligent Completion Design Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the ICV sizing for a zone with high flow requirements and a water shut-off objective."

**🤖 AI Agent:**
> The required valve configuration for the zone is a 3.5-inch Multi-Position valve to manage the high flow rate and precise choking needed for water shut-off.

---

**👤 You:**
> "How many control lines are needed for a 3000m well with 4 zones and 5 sensors?"

**🤖 AI Agent:**
> For a well of this depth and configuration, you will need 9 control lines in total.

---

**👤 You:**
> "What is the required HPU pressure for these valve requirements?"

**🤖 AI Agent:**
> The required operating pressure for the Hydraulic Power Unit is 4500 psi to ensure successful actuation.


## ❓ FAQ

**Q: How do I determine the correct valve size?**
You can use the `calculate_icv_sizing` tool, providing the zonal properties and your specific control objectives.

**Q: Can I design the monitoring layout for my well?**
Yes, the `generate_monitoring_layout` tool designs sensor placement based on your zonal properties and objectives.

**Q: What information is needed to size the HPU?**
To use `size_hpu`, you must provide the ICV requirements and the specifications for the control lines.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/intelligent-completion-design-engine](https://vinkius.com/en/ai-agent-connect/intelligent-completion-design-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Intelligent Completion Design Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `intelligent-completion-design-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Intelligent Completion Design Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "intelligent-completion-design-engine": {
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
