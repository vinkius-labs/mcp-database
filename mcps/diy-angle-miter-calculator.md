# DIY Angle Miter Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/diy-angle-miter-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [calculation](../categories/calculation.md)

Calculate exact miter and bevel angles for woodworking joints like baseboards and crown molding.

## Description
This MCP server provides precise calculations for woodworking projects. Use `get_flat_miter_settings` to determine the rotation needed for flat joints like baseboards or picture frames. For more complex tasks, `get_compound_miter_settings` calculates both miter and bevel angles for crown molding based on the spring angle. Finally, use `format_angle_to_dms` to convert decimal degrees into a human-readable format (degrees and minutes) that matches professional miter saw markings.


## Available Tools (3)
- **get_compound_molding_settings**: Calculates both the miter and bevel angles for crown molding
- **get_flat_miter_settings**: Calculates the necessary miter angle for simple flat joints
- **format_angle_to_dms**: g., 45° 30').

Converts a decimal degree value into a human-readable string


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DIY Angle Miter Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the miter angle for a 90 degree outside corner baseboard?"

**🤖 AI Agent:**
> The miter angle is 45.0 degrees.

---

**👤 You:**
> "Calculate the settings for crown molding with a 45 degree corner angle and a 38 degree spring angle at an inside corner."

**🤖 AI Agent:**
> Miter Angle: 31.62 degrees, Bevel Angle: 33.86 degrees.

---

**👤 You:**
> "Convert 45.5 degrees to degrees and minutes."

**🤖 AI Agent:**
> 45° 30'


## ❓ FAQ

**Q: How do I calculate angles for crown molding?**
Use the `get_compound_molding_settings` tool by providing the corner angle, the spring angle of your molding, and whether it is an inside or outside corner.

**Q: Can I use this for simple baseboards?**
Yes, use `get_flat_miter_settings` for any flat joint where no blade tilt is required.

**Q: How are the results formatted?**
You can use `format_angle_to_dms` to convert decimal degrees into a format like 45° 30' for easy reading on your saw.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/diy-angle-miter-calculator](https://vinkius.com/mcp/diy-angle-miter-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DIY Angle Miter Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `diy-angle-miter-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DIY Angle Miter Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "diy-angle-miter-calculator": {
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
