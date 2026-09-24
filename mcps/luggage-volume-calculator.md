# Luggage Volume Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/luggage-volume-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Calculate luggage volume and check airline compliance.

## Description
This MCP server provides precise tools for travelers to calculate the three-dimensional volume of their luggage. Use `get_volume_by_metric_dimensions` or `get_volume_by_imperial_dimensions` to find the volume in cm3 or in3, or use `get_volume_in_liters` for capacity in liters. You can also use `compare_to_limit` to verify if your bag meets specific airline requirements.


## Available Tools (4)
- **get_volume_by_metric_dimensions**: Calculates the volume of luggage using metric units (centimeters)
- **get_volume_by_imperial_dimensions**: Calculates the volume of luggage using imperial units (inches)
- **get_volume_in_liters**: Converts metric dimensions into liters
- **compare_to_limit**: Determines if a piece of luggage exceeds a specific volume threshold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Luggage Volume Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the volume of a bag that is 50cm x 30cm x 20cm?"

**🤖 AI Agent:**
> The volume of the bag is 30,000 cm3.

---

**👤 You:**
> "Convert a 20x15x10 inch bag to cubic inches."

**🤖 AI Agent:**
> The volume of the bag is 3,000 in3.

---

**👤 You:**
> "Is a 45 liter bag within a 50 liter limit?"

**🤖 AI Agent:**
> Yes, the bag is within the limit.


## ❓ FAQ

**Q: What units are supported?**
The server supports both metric (centimeters) and imperial (inches) units for dimension inputs.

**Q: Can I check if my bag is too big for an airline?**
Yes, you can use the `compare_to_limit` tool to check your calculated volume against an airline's maximum allowed volume.

**Q: How do I get the volume in liters?**
You can use the `get_volume_in_liters` tool by providing the length, width, and height in centimeters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/luggage-volume-calculator](https://vinkius.com/en/ai-agent-connect/luggage-volume-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Luggage Volume Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `luggage-volume-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Luggage Volume Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "luggage-volume-calculator": {
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
