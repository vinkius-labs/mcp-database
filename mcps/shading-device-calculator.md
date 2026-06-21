# Shading Device Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shading-device-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate precise dimensions for horizontal and vertical solar shading devices.

## Description
This MCP server provides specialized tools for architectural thermal comfort. Use `get_solar_position` to determine the sun's altitude and azimuth, then use `calculate_horizontal_depth` to find the minimum projection required for horizontal louvers or `calculate_vertical_width` for vertical fins. You can also audit existing structures using `validate_compliance` to ensure they meet your target solar cutoff angles.


## Available Tools
- **calculate_vertical_width**: Calculate minimum width for vertical fins
- **validate_compliance**: Validate shading device compliance
- **calculate_horizontal_depth**: Calculate minimum depth for horizontal louvers
- **get_solar_position**: Calculate the sun position


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shading Device Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the sun's position at latitude 40.7128 on day 150 at 12:00?"

**🤖 AI Agent:**
> By calling `get_solar_position`, the tool will return the specific solar altitude and azimuth for that location and time.

---

**👤 You:**
> "Calculate required depth for a horizontal louver at latitude 40, surface azimuth 180, solar altitude 45, solar azimuth 135, and cutoff angle 60."

**🤖 AI Agent:**
> The `calculate_horizontal_depth` tool will compute the minimum projection depth needed to satisfy the 60-degree cutoff requirement.

---

**👤 You:**
> "Check if a 0.5m depth louver is compliant with a 45 degree target angle."

**🤖 AI Agent:**
> The `validate_compliance` tool will analyze the geometry and return whether the device meets the design threshold or if there is a failure margin.


## ❓ FAQ

**Q: What does the calculator determine?**
It calculates the minimum depth for horizontal louvers and the maximum width for vertical fins needed to block sunlight based on solar trigonometry.

**Q: How do I use the compliance tool?**
Use `validate_compliance` by providing your current device dimensions, solar position, and target cutoff angle to check if the shading is effective.

**Q: What inputs are required for solar position?**
You need the latitude of the site, the day of the year, and the time of day in HH:mm format.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shading-device-calculator](https://vinkius.com/mcp/shading-device-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shading Device Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `shading-device-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shading Device Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shading-device-calculator": {
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
