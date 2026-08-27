# Sediment Basin Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sediment-basin-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design erosion control sediment basins using settling theory and NRCS standards.

## Description
This MCP server provides specialized engineering tools for designing sediment basins for erosion control. It uses sediment settling theory and NRCS design criteria to calculate physical dimensions, evaluate particle capture performance, and predict maintenance needs. Use `calculate_basin_dimensions` to determine volume and area, `estimate_settling_performance` to verify particle capture, `calculate_cleanout_schedule` for maintenance planning, and `validate_nrcs_compliance` to ensure safety standards are met.


## Available Tools (4)
- **estimate_settling_performance**: Evaluates if the designed basin can meet the trapping efficiency for specific particle sizes
- **calculate_basin_dimensions**: Determines the physical size requirements (volume, area, depth) of the basin
- **calculate_cleanout_schedule**: Predicts how often the basin must be emptied of sediment
- **validate_nrcs_compliance**: Checks if the proposed basin design adheres to NRCS safety and stability standards


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sediment Basin Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the dimensions for a basin with a 50 acre drainage area and a 2-inch design storm."

**🤖 AI Agent:**
> The required basin volume is 12,500 cubic meters with a surface area of 4,200 square meters and a maximum depth of 3.5 meters.

---

**👤 You:**
> "Will a basin with 500 square meters of surface area capture 0.05mm particles with a 24-hour detention time?"

**🤖 AI Agent:**
> Yes, the capture probability for 0.05mm particles is 85% given the current surface area and detention time.

---

**👤 You:**
> "Check if a basin with 2m depth and 2:1 side slopes is NRCS compliant."

**🤖 AI Agent:**
> The design is compliant with NRCS standards for the provided depth and side slope ratio.


## ❓ FAQ

**Q: How do I ensure my basin meets safety standards?**
You can use the `validate_nrcs_compliance` tool to check if your design adheres to NRCS safety and stability standards regarding depth, side slopes, and freeboard.

**Q: Can I calculate how often the basin needs cleaning?**
Yes, the `calculate_cleanout_schedule` tool predicts the interval between required maintenance events based on annual sediment yield and basin volume.

**Q: How is the basin size determined?**
The `calculate_basin_dimensions` tool determines the required volume, surface area, and depth based on your drainage area, design storm, and target trapping efficiency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sediment-basin-designer](https://vinkius.com/ai-agent-connect/sediment-basin-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sediment Basin Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sediment-basin-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sediment Basin Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sediment-basin-designer": {
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
