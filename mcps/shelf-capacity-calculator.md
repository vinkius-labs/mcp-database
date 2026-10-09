# Shelf Capacity Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/shelf-capacity-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [organization](../categories/organization.md)

Calculate how many objects fit on a shelf and the remaining space.

## Description
This MCP server provides precise spatial calculations for shelf organization. Use `calculate_shelf_capacity` to find the maximum number of whole objects that fit on a shelf and the leftover space, or `get_capacity_report` for a detailed utilization summary. It also includes `validate_shelf_dimensions` to ensure physical viability and `compare_shelf_configurations` to determine which setup accommodates more items.


## Available Tools (4)
- **calculate_shelf_capacity**: Determines how many whole objects fit on a shelf and how much space remains
- **compare_shelf_configurations**: Compares two different shelf setups to see which accommodates more objects
- **get_capacity_report**: Provides a detailed summary of the shelf utilization for a specific configuration
- **validate_shelf_dimensions**: Checks if a proposed set of dimensions is physically viable for any object placement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shelf Capacity Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many 15cm wide books can I fit on a 100cm shelf?"

**🤖 AI Agent:**
> You can fit 6 books on the shelf, with 10cm of remaining space.

---

**👤 You:**
> "Give me a report for a 500cm shelf with 20cm wide objects."

**🤖 AI Agent:**
> The shelf can hold 25 objects. The total occupied space is 500cm, leaving 0cm of remaining space, resulting in 100% utilization.

---

**👤 You:**
> "Is a 50cm shelf viable for 60cm wide objects?"

**🤖 AI Agent:**
> No, the configuration is not viable because the object width exceeds the shelf length.


## ❓ FAQ

**Q: How is capacity calculated?**
Capacity is the largest integer of whole objects that can fit within the total shelf length without exceeding it.

**Q: Can I compare two different shelf setups?**
Yes, you can use `compare_shelf_configurations` to see which setup accommodates more objects or has more remaining space.

**Q: What happens if the object is wider than the shelf?**
The tool will return an error indicating that the configuration is not physically viable.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/shelf-capacity-calculator](https://vinkius.com/en/ai-agent-connect/shelf-capacity-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shelf Capacity Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shelf-capacity-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shelf Capacity Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shelf-capacity-calculator": {
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
