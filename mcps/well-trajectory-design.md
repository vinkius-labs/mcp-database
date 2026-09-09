# Well Trajectory Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/well-trajectory-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design and validate precise wellbore paths for directional and horizontal drilling.

## Description
This MCP server provides specialized engineering tools for designing wellbore trajectories. It allows AI agents to generate complete paths from surface to target using methods like `minimum_curvature`. Users can validate designs using `validate_mechanical_constraints` to check for torque and drag, ensure safety with `check_anti_collision`, and decompose drilling phases using `analyze_build_and_hold`.


## Available Tools (4)
- **analyze_build_and_hold**: Decomposes the trajectory to identify specific drilling phases
- **check_anti_collision**: Ensures the new well trajectory does not intersect with existing nearby wells
- **design_trajectory**: Generates a complete wellbore path from surface to target
- **validate_mechanical_constraints**: Checks if the designed trajectory is physically drillable by evaluating friction and stress


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Well Trajectory Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Design a directional well from surface (0,0,0) to target (500,500,1000) with a max DLS of 3 degrees per 30m using minimum curvature."

**🤖 AI Agent:**
> The designed trajectory has a total measured depth of 1245.6 meters with a final inclination of 42.3 degrees and an azimuth of 45.0 degrees.

---

**👤 You:**
> "Check if this trajectory is drillable with a drill string weighing 5000kg and a friction coefficient of 0.25."

**🤖 AI Agent:**
> The trajectory is feasible. The maximum torque is 12500 Nm and the maximum drag is 4500 kg.

---

**👤 You:**
> "Analyze the drilling phases for the current trajectory."

**🤖 AI Agent:**
> The trajectory consists of a build section from 0 to 450m, a tangent section from 450 to 800m, and a horizontal section starting at 800m.


## ❓ FAQ

**Q: How do I design a new wellbore path?**
You can use the `design_trajectory` tool by providing the surface and target coordinates, the well type, and the maximum allowable dogleg severity.

**Q: Can I check if my design will cause mechanical issues?**
Yes, the `validate_mechanical_constraints` tool evaluates friction and stress to determine if the trajectory is physically drillable.

**Q: How does the tool prevent collisions with existing wells?**
The `check_anti_collision` tool compares the new trajectory against a list of existing well paths to identify any potential intersection risks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/well-trajectory-design](https://vinkius.com/ai-agent-connect/well-trajectory-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Well Trajectory Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `well-trajectory-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Well Trajectory Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "well-trajectory-design": {
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
