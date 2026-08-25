# Depth of Field Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/depth-of-field-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Deterministic photographic engine for depth of field, hyperfocal distance, and sensor equivalence.

## Description
This MCP server provides a deterministic engine for precise photographic calculations. It connects AI agents to professional optical math, allowing for the calculation of near and far focus limits, total depth of field, and hyperfocal distance. The engine automatically switches between standard and macro magnification models based on focus distance. Use `calculate_dof` for primary depth of field metrics, `calculate_hyperfocal` to find the hyperfocal distance, and `get_sensor_equivalence` to adjust the Circle of Confusion for different sensor formats like APS-C or Micro 4/3.


## Available Tools (3)
- **get_sensor_equivalence**: Adjusts the Circle of Confusion based on different sensor formats to allow for crop factor comparisons
- **calculate_dof**: Calculates the primary depth of field metrics for a given photographic setup
- **calculate_hyperfocal**: Determines the hyperfocal distance for a specific lens and aperture setting


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Depth of Field Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the depth of field for a 50mm lens at f/2.8 with a focus distance of 2 meters using metric units."

**🤖 AI Agent:**
> The total depth of field is 0.24 meters, with a near limit of 1.82 meters and a far limit of 2.06 meters.

---

**👤 You:**
> "What is the hyperfocal distance for a 35mm lens at f/8 with a CoC of 0.029mm?"

**🤖 AI Agent:**
> The hyperfocal distance is 19.11 meters.

---

**👤 You:**
> "What is the crop factor and equivalent CoC for an APS-C sensor compared to a full-frame sensor with a base CoC of 0.029?"

**🤖 AI Agent:**
> The crop factor is 1.5 and the equivalent CoC is 0.0193mm.


## ❓ FAQ

**Q: How does the tool handle macro photography?**
The `calculate_dof` tool automatically detects macro scenarios. If the focus distance is less than ten times the focal length, it switches from the standard formula to a magnification-based formula for higher accuracy.

**Q: Can I calculate sensor crop factors?**
Yes, you can use `get_sensor_equivalence` to determine the equivalent Circle of Confusion and the crop factor for various sensor formats including APS-C and Micro 4/3.

**Q: What is hyperfocal distance?**
Hyperfocal distance is the closest distance at which a lens can be focused while keeping objects from that distance to infinity acceptably sharp. You can find this value using `calculate_hyperfocal`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/depth-of-field-calculator](https://vinkius.com/ai-agent-connect/depth-of-field-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Depth of Field Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `depth-of-field-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Depth of Field Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "depth-of-field-calculator": {
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
