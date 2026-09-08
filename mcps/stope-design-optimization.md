# Stope Design Optimization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/stope-design-optimization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Optimize underground stope geometries using rock mechanics and stability analysis.

## Description
This MCP server provides specialized tools for underground mining engineers to design optimal stope geometries. By integrating ore body geometry with rock mass properties, the server allows for precise stability assessments and extraction planning. Use `analyze_stope_stability` to verify if a proposed void is safe, `calculate_optimal_dimensions` to find the best size within ore body bounds, and `get_extraction_ratio` to quantify recovered volume. It also includes `generate_stability_chart` for sensitivity analysis across different rock mass ratings and wall angles.


## Available Tools (4)
- **analyze_stope_stability**: Determines if a proposed stope geometry is physically stable based on rock mass properties
- **calculate_optimal_dimensions**: Suggests the most efficient stope dimensions that maximize extraction without exceeding safety limits
- **get_extraction_ratio**: Calculates the percentage of the ore body being extracted relative to the total available volume
- **generate_stability_chart**: Provides a summary of stability outcomes across various potential stope sizes to aid in sensitivity analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stope Design Optimization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is a stope with dimensions 20x10x15, RMR of 65, a 70 degree hanging wall, and a 75 degree footwall stable?"

**🤖 AI Agent:**
> The stope is stable with a stability factor of 1.45 and a low failure risk.

---

**👤 You:**
> "What are the optimal dimensions for an ore body with bounds minX:0, maxX:50, minY:0, maxY:30, minZ:0, maxZ:20, an RMR of 50, and a target dilution limit of 10%?"

**🤖 AI Agent:**
> The optimal dimensions are 35m length, 12m width, and 15m height, with a predicted dilution of 8.5%.

---

**👤 You:**
> "Calculate the extraction ratio for a stope of 15x10x10 in an ore body with a volume of 5000 cubic meters."

**🤖 AI Agent:**
> The extraction ratio is 3.0%, with a recovered volume of 1500 cubic meters and 3500 cubic meters of wasted volume.


## ❓ FAQ

**Q: How do I check if my stope design is safe?**
You can use the `analyze_stope_stability` tool. Provide the stope dimensions, the Rock Mass Rating (RMR), and the hanging wall and footwall angles to receive a stability factor and risk assessment.

**Q: Can I find the best dimensions to maximize ore recovery?**
Yes, the `calculate_optimal_dimensions` tool suggests efficient dimensions that maximize extraction while staying within your target dilution limits and ore body boundaries.

**Q: How is the extraction ratio calculated?**
The `get_extraction_ratio` tool calculates the percentage of the total ore body volume that is successfully recovered based on your proposed stope dimensions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/stope-design-optimization](https://vinkius.com/ai-agent-connect/stope-design-optimization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stope Design Optimization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stope-design-optimization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stope Design Optimization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stope-design-optimization": {
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
