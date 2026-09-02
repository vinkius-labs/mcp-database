# Extraction Column Design Tool MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/extraction-column-design-tool)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design liquid-liquid extraction columns by calculating stages, diameter, height, and hydrodynamics.

## Description
This MCP server provides a complete suite of engineering tools for designing liquid-liquid extraction columns. It allows AI agents to perform complex chemical engineering calculations, including determining the `get_theoretical_stages` required for specific separation targets, calculating the `calculate_column_diameter` to prevent flooding, and determining the `calculate_column_height` based on stage efficiency. Additionally, users can `evaluate_hydrodynamics` to assess phase dispersion and coalescence tendencies, ensuring stable column operation.


## Available Tools (4)
- **evaluate_hydrodynamics**: Assess the stability of the extraction by analyzing dispersion and coalescence tendencies
- **calculate_column_diameter**: Determine the required diameter of the column to prevent flooding based on phase flow rates
- **calculate_column_height**: Determine the physical height of the column required to accommodate the necessary stages
- **get_theoretical_stages**: Determine the minimum number of contact stages required to meet a specific separation target


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Extraction Column Design Tool** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many stages do I need for a feed concentration of 0.5, solvent concentration of 0.1, and a target concentration of 0.05 using this equilibrium data: {"points": [[0.1, 0.05], [0.5, 0.2]]}?"

**🤖 AI Agent:**
> The required number of theoretical stages is 4, with a calculated solvent-to-feed ratio of 1.5.

---

**👤 You:**
> "Calculate the column diameter for a feed flow of 10 m3/h, solvent flow of 5 m3/h, feed density of 1000 kg/m3, solvent density of 800 kg/m3, and interfacial tension of 0.02 N/m."

**🤖 AI Agent:**
> The required column diameter is 1.25 meters with a flooding margin of 0.25.

---

**👤 You:**
> "What is the total height for 5 theoretical stages with 0.7 efficiency and 0.5m tray spacing?"

**🤖 AI Agent:**
> The total height of the column is 3.57 meters, with an active height of 2.5 meters.


## ❓ FAQ

**Q: What can I calculate with this tool?**
You can calculate the number of theoretical stages, the required column diameter to avoid flooding, the total column height, and evaluate hydrodynamic stability like dispersion and coalescence.

**Q: How do I prevent column flooding?**
Use the `calculate_column_diameter` tool with your feed and solvent flow rates, densities, and interfacial tension to find the optimal diameter that maintains a safe flooding margin.

**Q: Does this tool account for stage efficiency?**
Yes, the `calculate_column_height` tool requires a stage efficiency parameter (0.0 to 1.0) to convert theoretical stages into the actual physical height needed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/extraction-column-design-tool](https://vinkius.com/ai-agent-connect/extraction-column-design-tool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Extraction Column Design Tool** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `extraction-column-design-tool` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Extraction Column Design Tool** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "extraction-column-design-tool": {
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
