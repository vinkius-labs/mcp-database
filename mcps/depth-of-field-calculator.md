# Depth of Field Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/depth-of-field-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate precise depth of field, hyperfocal distance, and blur limits for any camera sensor.

## Description
An advanced optical utility for photographers to determine focus boundaries. Use `lookup_camera` to find sensor-specific crop factors and CoC limits, then use `calculate_dof_metrics` to compute near/far limits and hyperfocal distance based on your lens settings.


## Available Tools (3)
- **lookup_camera**: Look up camera properties
- **calculate_dof_metrics**: Calculate depth of field metrics
- **convert_units**: g., mm to m).

Convert measurement units


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Depth of Field Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the depth of field for a 50mm lens at f/2.8 on a Sony A7IV at 2 meters distance?"

**🤖 AI Agent:**
> For a Sony A7IV (Full Frame), the near limit is 1.85m and the far limit is 2.16m, providing a total depth of field of 0.31m.

---

**👤 You:**
> "Find the hyperfocal distance for an 85mm lens at f/1.8 on a Canon EOS R7."

**🤖 AI Agent:**
> The hyperfocal distance for your Canon EOS R7 setup is approximately 12.45 meters.

---

**👤 You:**
> "Convert 0.05 meters to inches."

**🤖 AI Agent:**
> 0.05 meters is approximately 1.97 inches.


## ❓ FAQ

**Q: How do I find the correct Circle of Confusion (CoC) for my camera?**
Use the `lookup_camera` tool with your specific camera model name to retrieve the precise CoC limit and crop factor from our database.

**Q: Can I calculate depth of field for macro photography?**
Yes. By providing a small `subjectDistance` and the appropriate `cocLimit` via `calculate_dof_metrics`, you can determine the extremely shallow depth of field typical in macro work.

**Q: What units are used for the results?**
The `calculate_dof_metrics` tool provides results in meters, feet, and inches. You can also use `convert_units` to transform any measurement between mm, cm, m, km, inch, or ft.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/depth-of-field-calculator](https://vinkius.com/mcp/depth-of-field-calculator)
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
