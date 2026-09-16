# Gas Measurement Station Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/gas-measurement-station-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design gas measurement stations with AGA-compliant meter selection, run lengths, and configurations.

## Description
This MCP server provides engineering tools to design gas measurement stations following AGA standards (Report No. 3, 7, and 9). It allows users to select the optimal meter technology, calculate required upstream and downstream pipe lengths, design physical station layouts, and establish calibration protocols. Use `select_meter_technology` to find the best fit for your flow and accuracy needs, `calculate_meter_run_length` to ensure stable flow, `design_station_configuration` for physical layouts, and `determine_calibration_protocol` to maintain precision.


## Available Tools (4)
- **design_station_configuration**: Provides a complete station layout specification including pressure and temperature measurement points
- **calculate_meter_run_length**: Determines the required length of straight piping needed for stable flow
- **determine_calibration_protocol**: Specifies the necessary verification and calibration steps to maintain the target accuracy
- **select_meter_technology**: Determines the most appropriate meter type based on the physical constraints and accuracy needs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gas Measurement Station Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What meter should I use for a flow rate of 500-1500 m3/h with high accuracy requirements?"

**🤖 AI Agent:**
> Based on your requirements, an Ultrasonic meter is recommended for high accuracy in this flow range.

---

**👤 You:**
> "Calculate the meter run length for an Orifice meter with a 6-inch pipe and no flow conditioner."

**🤖 AI Agent:**
> For a 6-inch pipe using an Orifice meter without a flow conditioner, you require 20 diameters of upstream length and 5 diameters of downstream length.

---

**👤 You:**
> "Design a station configuration for an Ultrasonic meter operating at 50 bar and 40 degrees Celsius."

**🤖 AI Agent:**
> The station configuration for your Ultrasonic meter includes specific placement for pressure and temperature transmitters to ensure accurate gas density calculations at 50 bar and 40°C.


## ❓ FAQ

**Q: Which AGA standards are supported?**
The tools support AGA Report No. 3 for orifice meters, AGA Report No. 7 for ultrasonic meters, and AGA Report No. 9 for turbine meters.

**Q: How do I determine the required pipe length?**
You can use the `calculate_meter_run_length` tool. It calculates the necessary upstream and downstream lengths based on the meter type, pipe diameter, and whether a flow conditioner is used.

**Q: Can I design a station for custody transfer?**
Yes. When using `determine_calibration_protocol`, you can specify if the application is for custody transfer to receive the appropriate high-precision verification steps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/gas-measurement-station-designer](https://vinkius.com/en/ai-agent-connect/gas-measurement-station-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gas Measurement Station Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gas-measurement-station-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gas Measurement Station Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gas-measurement-station-designer": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
