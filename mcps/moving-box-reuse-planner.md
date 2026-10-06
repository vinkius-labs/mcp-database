# Moving Box Reuse Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moving-box-reuse-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate moving box needs and rental costs based on room inventory and existing boxes.

## Description
This MCP server helps optimize moving logistics by calculating the exact volume of items in your rooms and comparing it against the capacity of boxes you already own. Use `generate_reuse_plan` to get a complete summary of your moving needs, or use `get_total_volume_needed` to find the total volume of your items. It also provides tools like `calculate_existing_capacity` to assess your current assets and `estimate_rental_requirements` to find the most cost-effective rental options for any remaining volume.


## Available Tools (4)
- **estimate_rental_requirements**: Determines how many new boxes must be rented and the associated costs
- **generate_reuse_plan**: Provides a complete summary of the moving needs, including existing assets and new requirements
- **get_total_volume_needed**: Determines the total physical volume required to house all items across all provided rooms
- **calculate_existing_capacity**: Calculates how much volume can be covered by the boxes the user already owns


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moving Box Reuse Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my moving needs for a living room with a sofa (volume 2.5) and a TV (volume 1.2), and I have one box with capacity 3.0."

**🤖 AI Agent:**
> You need a total volume of 3.7. With your existing capacity of 3.0, you have a shortfall of 0.7. You will need to rent additional boxes to cover the remaining volume.

---

**👤 You:**
> "What is the total volume for these items: a chair (0.5) and a table (2.0)?"

**🤖 AI Agent:**
> The total volume required is 2.5.

---

**👤 You:**
> "How much capacity do I have if I own two boxes with capacities of 1.5 and 2.5?"

**🤖 AI Agent:**
> Your total existing capacity is 4.0.


## ❓ FAQ

**Q: How does the tool calculate the total volume?**
The `get_total_volume_needed` tool sums the volume of every individual item provided in your room inventories.

**Q: Can I see how many boxes I need to rent?**
Yes, you can use `estimate_rental_requirements` to determine the number of boxes to rent and the total cost based on available box types.

**Q: What is a reuse plan?**
A reuse plan, generated via `generate_reuse_plan`, provides a full summary including total volume needed, existing capacity, and the specific rental plan required to cover the shortfall.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moving-box-reuse-planner](https://vinkius.com/en/ai-agent-connect/moving-box-reuse-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moving Box Reuse Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moving-box-reuse-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moving Box Reuse Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moving-box-reuse-planner": {
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
