# Terrace Design Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/terrace-design-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Design erosion control terrace systems using NRCS standards.

## Description
This MCP server provides specialized tools for designing terrace systems to mitigate soil erosion on sloped terrain. By following NRCS principles, it allows users to calculate optimal terrace spacing, determine terrace grade and channel capacity, design stable outlets, and estimate the required earthwork volume. Use `calculate_spacing` to find the distance between terraces, `calculate_grade_and_capacity` to define water movement, `design_outlet` to ensure downstream stability, and `estimate_earthwork` to plan construction volumes.


## Available Tools (4)
- **calculate_grade_and_capacity**: Defines the longitudinal slope of the terrace and its ability to carry water
- **calculate_spacing**: Determines the optimal distance between terraces to prevent erosion
- **design_outlet**: Specifies the requirements for the water exit point to ensure downstream stability
- **estimate_earthwork**: Calculates the volume of soil movement required for construction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Terrace Design Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the terrace spacing for a slope with a 5% gradient, 100m length, erodibility of 0.3, rainfall intensity of 50mm/hr, and a crop rotation factor of 1.2 using broadbase terraces."

**🤖 AI Agent:**
> The required terrace spacing is 25.5 meters with a safety factor of 1.15.

---

**👤 You:**
> "How much earthwork volume is needed for a 150m slope with 30m spacing, using steep_backslope terraces and an average depth of 0.5m?"

**🤖 AI Agent:**
> The estimated total earthwork volume is 187.5 cubic meters with a cut/fill ratio of 1.0.

---

**👤 You:**
> "Design an outlet for a system with a channel capacity of 500 L/s and a max flow rate of 450 L/s, where downstream sensitivity is 0.8."

**🤖 AI Agent:**
> The recommended outlet type is a Riprap Apron with required dimensions of 2m x 3m and a velocity limit of 1.5 m/s.


## ❓ FAQ

**Q: What standards does this tool follow?**
The design logic follows NRCS (Natural Resources Conservation Service) principles for soil and water conservation.

**Q: How do I determine the distance between terraces?**
You can use the `calculate_spacing` tool, providing the slope gradient, length, soil erodibility, rainfall intensity, and crop rotation factor.

**Q: Can I design different types of terraces?**
Yes, the tools support both broadbase terraces for gentle slopes and steep backslope terraces for steeper terrain.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/terrace-design-calculator](https://vinkius.com/ai-agent-connect/terrace-design-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Terrace Design Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `terrace-design-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Terrace Design Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "terrace-design-calculator": {
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
