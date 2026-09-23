# Seed Depth Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/seed-depth-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Convert planting depths between metric and imperial units and validate seed depth ranges.

## Description
This MCP server provides essential tools for agricultural and gardening precision. It allows AI agents to perform accurate conversions between millimeters, centimeters, meters, and inches using `convert_depth`. Users can also verify if a specific planting depth is appropriate for various plant categories, such as microgreens or trees, using `validate_depth_range`. It ensures planting accuracy to prevent seed desiccation or insufficient energy for surface emergence.


## Available Tools (4)
- **validate_depth_range**: Is this specific depth appropriate for a given seed type?
- **list_supported_units**: Which length units can I use for conversion?
- **convert_depth**: Converts planting depth between supplied length units
- **get_unit_conversion_factor**: What is the ratio between unit A and unit B?


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Seed Depth Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert 5 centimeters to inches."

**🤖 AI Agent:**
> 5 centimeters is approximately 1.97 inches.

---

**👤 You:**
> "Is a depth of 2mm okay for microgreens?"

**🤖 AI Agent:**
> Yes, 2mm is within the safe range for microgreens.

---

**👤 You:**
> "What is 0.5 meters in millimeters?"

**🤖 AI Agent:**
> 0.5 meters is 500 millimeters.


## ❓ FAQ

**Q: What units are supported for conversion?**
The server supports millimeters (mm), centimeters (cm), meters (m), and inches (in).

**Q: How can I check if a depth is safe for my seeds?**
You can use the `validate_depth_range` tool by providing the depth and the seed type, such as 'vegetable' or 'microgreen'.

**Q: Can I convert between any two supported units?**
Yes, you can use `convert_depth` to translate any value between the supported units like mm, cm, m, or in.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/seed-depth-converter](https://vinkius.com/en/ai-agent-connect/seed-depth-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Seed Depth Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `seed-depth-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Seed Depth Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "seed-depth-converter": {
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
