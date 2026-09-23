# Garden Area Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/garden-area-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Calculate garden bed areas and estimate material volumes and costs.

## Description
This MCP server provides tools to manage garden dimensions and material planning. Use `get_rectangular_area` and `get_circular_area` to find the surface area of your beds. Once the area is known, use `calculate_material_volume` to determine how much soil or mulch is required based on depth, and `estimate_material_cost` to find the total price for your supplies.


## Available Tools (4)
- **get_circular_area**: 
- **calculate_material_volume**: 
- **estimate_material_cost**: 
- **get_rectangular_area**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Garden Area Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the area of a rectangular garden that is 5 meters long and 3 meters wide?"

**🤖 AI Agent:**
> The area of the rectangular garden is 15 square meters.

---

**👤 You:**
> "I have a circular garden with a radius of 2 meters. How much area does it cover?"

**🤖 AI Agent:**
> The circular garden covers approximately 12.57 square meters.

---

**👤 You:**
> "How much soil do I need for a 10 square meter area with a depth of 0.2 meters?"

**🤖 AI Agent:**
> You will need 2 cubic meters of soil.


## ❓ FAQ

**Q: How do I calculate the area of my rectangular garden?**
You can use the `get_rectangular_area` tool by providing the length and width of your garden bed.

**Q: Can I estimate the cost of mulch?**
Yes, after calculating the required volume, use `estimate_material_cost` with your local unit price to get the total cost.

**Q: What units are supported?**
The tools work with any consistent units you provide, such as meters or feet, as long as you remain consistent across calculations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/garden-area-calculator](https://vinkius.com/en/ai-agent-connect/garden-area-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Garden Area Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `garden-area-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Garden Area Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "garden-area-calculator": {
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
