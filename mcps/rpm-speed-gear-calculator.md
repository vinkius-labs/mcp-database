# RPM & Speed Gear Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rpm-speed-gear-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate engine RPM at specific vehicle speeds or predict speed from a given RPM.

## Description
This MCP server provides precise mechanical calculations for manual transmission vehicles. Use `get_gear_rpm` to find the exact engine revolutions per minute for a specific gear, or use `get_all_gears_at_speed` to see an RPM report across your entire gear range at a target velocity. You can also predict vehicle speed using `calculate_speed_from_rpm`. All calculations account for tire diameter and final drive ratios.


## Available Tools (3)
- **get_gear_rpm**: Determines the exact engine revolutions per 1 minute for a single specific gear at a desired speed
- **calculate_speed_from_rpm**: Predicts what the vehicle's speed will be if the driver maintains a specific engine RPM in a chosen gear
- **get_all_gears_at_speed**: Provides a comprehensive overview of the engine's RPM across every available gear in the transmission at a single target speed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RPM & Speed Gear Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What will my RPM be in 4th gear at 65 MPH if my tire diameter is 26 inches, gear ratio is 1.0, and final drive is 3.73?"

**🤖 AI Agent:**
> At 65 MPH with a 26-inch tire, your engine RPM in 4th gear will be approximately 3185 RPM.

---

**👤 You:**
> "Calculate the speed for 3000 RPM in 3rd gear (ratio 1.3, final drive 3.5) with 25 inch tires."

**🤖 AI Agent:**
> Maintaining 3000 RPM in 3rd gear will result in a vehicle speed of approximately 41.6 MPH.

---

**👤 You:**
> "Show me the RPM for all gears (3.5, 2.1, 1.4, 1.0) at 100 KMH with a 600mm tire and 4.1 final drive."

**🤖 AI Agent:**
> At 100 KMH, the RPM report is: 1st gear: 3852, 2nd gear: 2287, 3rd gear: 1574, 4th gear: 1169.


## ❓ FAQ

**Q: How do I calculate RPM for a specific gear?**
You can use the `get_gear_rpm` tool by providing the target speed, tire diameter, gear ratio, and final drive ratio.

**Q: Can I see RPM for all gears at once?**
Yes, the `get_all_gears_at_speed` tool generates a comprehensive report showing the RPM for every gear ratio provided in your list.

**Q: Does this support metric units?**
Yes, the tools support KMH for speed and MM for tire diameter, alongside MPH and INCH.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rpm-speed-gear-calculator](https://vinkius.com/mcp/rpm-speed-gear-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RPM & Speed Gear Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rpm-speed-gear-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RPM & Speed Gear Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rpm-speed-gear-calculator": {
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
