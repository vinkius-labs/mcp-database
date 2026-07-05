# Moving Truck Sizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moving-truck-sizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate the exact truck size needed for your move based on home type and bulky items.

## Description
Plan your relocation with precision using the Moving Truck Sizer. This tool calculates the total estimated cubic footage required for your move by analyzing your residential profile--such as studio, 1-bed, or 4-bed homes--and the square footage of your property. It also accounts for high-volume items like pianos, sectional sofas, and appliances using the `estimate_volume` tool. Once you have your volume estimate, use `recommend_truck` to find the most efficient vehicle from our fleet, including Cargo Vans, 10ft, 15ft, 20ft, or 26ft trucks. The system applies a safety buffer rule, ensuring you never exceed 90% of a truck's capacity, and will even suggest an upgrade via `recommend_truck` if your load is too dense for the selected size. You can also browse the full fleet using `get_truck_inventory`.


## Available Tools (3)
- **recommend_truck**: Recommend the best truck size based on estimated volume
- **estimate_volume**: Calculate the total estimated cubic footage required for a move
- **get_truck_inventory**: Get the list of available trucks and their capacities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moving Truck Sizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am moving from a 1200 sq ft 2-bed apartment and I have a piano and a sectional sofa. How much space will I need?"

**🤖 AI Agent:**
> Based on your 2-bed apartment and bulky items, the estimated volume is approximately 850 cubic feet. This fits best in a 15ft truck.

---

**👤 You:**
> "What is the capacity of the largest truck available?"

**🤖 AI Agent:**
> The largest vehicle in our fleet is the 26ft truck, which has a maximum capacity of 1600 cubic feet.

---

**👤 You:**
> "I have an estimated volume of 1500 cubic feet. Which truck should I use?"

**🤖 AI Agent:**
> For a volume of 1500 cubic feet, the 26ft truck is recommended. Note that this exceeds the 90% safety threshold for this size, so please ensure your items are packed efficiently.


## ❓ FAQ

**Q: How does the volume estimation work?**
The `estimate_volume` tool calculates a base volume using your home's square footage and type, then adds specific volume penalties for each bulky item like a piano or king bed listed in your inventory.

**Q: What happens if my items exceed the truck capacity?**
The `recommend_truck` tool enforces a 90% safety buffer. If your estimated volume exceeds 90% of a truck's capacity, the system will automatically suggest moving up to the next larger vehicle tier.

**Q: Can I see all available truck sizes?**
Yes, you can use the `get_truck_inventory` tool to retrieve the complete list of our authorized fleet, including capacities for Cargo Vans up to 26ft trucks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moving-truck-sizer](https://vinkius.com/mcp/moving-truck-sizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moving Truck Sizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moving-truck-sizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moving Truck Sizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moving-truck-sizer": {
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
