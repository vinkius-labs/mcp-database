# Perforation Design Optimization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/perforation-design-optimization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Optimizes perforation geometry and density for oil and gas well completions.

## Description
This MCP server provides specialized engineering tools to optimize perforation designs in oil and gas well completions. It calculates ideal perforation density, phasing, and penetration depth based on formation strength and sand control requirements. Users can use `optimize_design_workflow` to find the best balance between reservoir productivity and wellbore stability, or use `validate_sand_stability` to ensure a design won't cause formation collapse. It also includes `estimate_productivity_impact` to predict performance relative to an ideal state.


## Available Tools (4)
- **calculate_perforation_geometry**: Determines the optimal physical characteristics of the perforation pattern
- **estimate_productivity_impact**: Predicts how the chosen design will perform relative to an ideal state
- **optimize_design_workflow**: An orchestration tool that iterates through design parameters to find the best balance between productivity and stability
- **validate_sand_stability**: Checks if the proposed perforation design will cause the formation to collapse or produce sand


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Perforation Design Optimization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the best perforation design for a formation with strength 0.8, strict sand control, a target productivity of 500, and a damaged zone radius of 0.2."

**🤖 AI Agent:**
> The optimal design features a perforation density of 4 shots per unit, 60 degree phasing, and a penetration depth of 0.5 units, ensuring stability with a safety margin of 0.15.

---

**👤 You:**
> "Calculate the perforation geometry for a rock with strength 0.5 and moderate sand control for a target productivity of 300."

**🤖 AI Agent:**
> The recommended geometry is 6 shots per unit, 90 degree phasing, and a penetration depth of 0.4 units.

---

**👤 You:**
> "Check if a design with density 12 and strength 0.3 is stable for strict sand control."

**🤖 AI Agent:**
> No, the design is unstable. The high perforation density in a low-strength formation exceeds the safety threshold.


## ❓ FAQ

**Q: How do I ensure my perforation design is stable?**
You can use the `validate_sand_stability` tool to check if your proposed density and formation strength meet safety requirements.

**Q: Can I automate the entire design process?**
Yes, the `optimize_design_workflow` tool automates the iteration through parameters to find the most productive design that remains safe.

**Q: What inputs are required for productivity estimation?**
To use `estimate_productivity_impact`, you need the geometry result, the damaged zone radius, and the underbalance pressure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/perforation-design-optimization](https://vinkius.com/en/ai-agent-connect/perforation-design-optimization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Perforation Design Optimization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `perforation-design-optimization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Perforation Design Optimization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "perforation-design-optimization": {
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
