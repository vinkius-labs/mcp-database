# Distillation Column Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/distillation-column-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design binary distillation columns by calculating stages, feed locations, and diameters.

## Description
This MCP server provides specialized chemical engineering tools for designing binary distillation columns. It allows AI agents to perform complex separation calculations using the McCabe-Thiele or Fenske-Underwood-Gilliland (FUG) methods. Users can determine the number of theoretical stages with `calculate_theoretical_stages`, convert them to physical trays using `calculate_actual_stages`, find the optimal entry point with `optimize_feed_location`, and size the column width via `estimate_column_diameter`.


## Available Tools (4)
- **calculate_actual_stages**: Converts theoretical equilibrium stages into the real-world number of physical trays needed
- **calculate_theoretical_stages**: Determines the number of equilibrium stages required for a specific separation
- **estimate_column_diameter**: Calculates the required physical width of the column to handle liquid and vapor loads
- **optimize_feed_location**: Identifies the most efficient tray to introduce the feed to the column


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Distillation Column Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the theoretical stages for a separation with a feed composition of 0.5, distillate of 0.95, bottoms of 0.05, relative volatility of 2.5, and a reflux ratio of 1.5 using McCabe-Thiele."

**🤖 AI Agent:**
> The required number of theoretical stages is 12, with a minimum reflux of 1.1 and the optimal feed stage located at stage 6.

---

**👤 You:**
> "I have 15 theoretical stages and a Murphree efficiency of 0.7. How many actual trays do I need?"

**🤖 AI Agent:**
> You will need 21 actual trays.

---

**👤 You:**
> "Find the optimal feed stage for 20 total stages, feed composition 0.4, distillate 0.9, and relative volatility 2.0."

**🤖 AI Agent:**
> The optimal feed stage is stage 11, providing a feed concentration match of 0.39.


## ❓ FAQ

**Q: Which calculation methods are supported?**
The server supports the McCabe-Thiele method for graphical/analytical stage determination and the Fenske-Underwood-Gilliland (FUG) shortcut method.

**Q: How do I account for real-world tray efficiency?**
You can use the `calculate_actual_stages` tool, which takes the theoretical stages and the Murphree efficiency to calculate the required physical trays.

**Q: Can I estimate the physical size of the column?**
Yes, the `estimate_column_diameter` tool calculates the required column diameter based on vapor flow, liquid flow, and flooding velocity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/distillation-column-designer](https://vinkius.com/ai-agent-connect/distillation-column-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Distillation Column Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `distillation-column-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Distillation Column Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "distillation-column-designer": {
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
