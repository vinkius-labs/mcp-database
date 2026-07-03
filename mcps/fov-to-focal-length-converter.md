# FOV to Focal Length Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fov-to-focal-length-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Convert between Field of View (degrees) and Focal Length (mm) for various sensor formats.

## Description
This MCP server provides precise mathematical conversions between horizontal Field of View (FOV) in degrees and lens focal length in millimeters. It supports multiple sensor formats including Full Frame, APS-C, Micro Four Thirds (M4/3), and 1-inch sensors. Use `calculate_focal_length_from_fov` to find the required lens for a specific angle, `calculate_fov_from_focal_length` to predict your view, or `get_sensor_equivalence` to understand crop factor magnification.


## Available Tools (3)
- **calculate_focal_length_from_fov**: Determine the required lens focal length for a target FOV
- **calculate_fov_from_focal_length**: Predict the horizontal field of view for a specific lens
- **get_sensor_equivalence**: Calculate crop factor and Full Frame equivalent focal length


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FOV to Focal Length Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What focal length do I need for a 45 degree FOV on an APS-C sensor?"

**🤖 AI Agent:**
> To achieve a 45-degree horizontal field of view on an APS-C sensor, you would need a lens with a focal length of approximately 32.18mm.

---

**👤 You:**
> "If I use a 50mm lens on a Micro Four Thirds sensor, what is the field of view?"

**🤖 AI Agent:**
> Using a 50mm lens on a Micro Four Thirds (M4/3) sensor results in a horizontal field of view of approximately 25.81 degrees.

---

**👤 You:**
> "What is the crop factor for a 1-inch sensor?"

**🤖 AI Agent:**
> The crop factor for a 1-inch sensor is approximately 2.3, meaning a lens will appear more magnified compared to Full Frame.


## ❓ FAQ

**Q: What sensor formats are supported?**
The tool supports Full Frame, APS-C, Micro Four Thirds (M4/3), and 1-inch sensors.

**Q: How do I calculate the crop factor?**
You can use the `get_sensor_equivalence` tool to automatically calculate the crop factor and the Full Frame equivalent focal length.

**Q: Does this account for vertical field of view?**
No, this tool specifically focuses on the horizontal Field of View (FOV) calculations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fov-to-focal-length-converter](https://vinkius.com/mcp/fov-to-focal-length-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FOV to Focal Length Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fov-to-focal-length-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FOV to Focal Length Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fov-to-focal-length-converter": {
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
