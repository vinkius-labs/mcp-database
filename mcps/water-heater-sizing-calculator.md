# Water Heater Sizing Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/water-heater-sizing-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate required First Hour Rating (FHR), tank capacity, and efficiency benchmarks for water heaters based on occupancy and fuel type.

## Description
This MCP server provides precise calculation tools for sizing water heating systems. Use `calculate_fhr_requirement` to determine the necessary First Hour Rating (FHR) based on occupant demand, usage type (residential or commercial), and fuel technology recovery rates. The `calculate_tank_capacity` tool recommends minimum tank volumes in gallons by analyzing occupancy patterns. Additionally, use `get_efficiency_comparison` to compare Energy Factor (EF) benchmarks across gas, electric, and heat pump technologies. This is essential for plumbing professionals and engineers planning efficient hot water delivery systems.


## Available Tools (3)
- **calculate_fhr_requirement**: Determines the required First Hour Rating (FHR) needed to meet demand
- **calculate_tank_capacity**: Determines the recommended minimum tank volume in gallons
- **get_efficiency_comparison**: Provides a comparative view of the Energy Factor expectations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Water Heater Sizing Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much FHR do I need for a residential house with 4 people using gas heating?"

**🤖 AI Agent:**
> For a residential setup with 4 occupants and gas heating, the required First Hour Rating (FHR) is 52 gallons per hour.

---

**👤 You:**
> "What is the recommended tank size for a commercial building with 20 people?"

**🤖 AI Agent:**
> For a commercial usage profile with 20 occupants, the recommended minimum tank capacity is 450 gallons.

---

**👤 You:**
> "Compare the efficiency of gas vs heat pump water heaters."

**🤖 AI Agent:**
> Heat pump technology offers a significantly higher Energy Factor (EF) range compared to traditional gas-fired units, making it more efficient for long-term energy savings.


## ❓ FAQ

**Q: How do I calculate the required FHR?**
Use the `calculate_frl_requirement` tool by providing the number of occupants, whether the usage is residential or commercial, and the heating fuel type (gas, electric, or heat pump).

**Q: What factors affect the tank capacity recommendation?**
The recommended capacity is based on the number of occupants and the usage type. Commercial profiles use a higher multiplier to account for more frequent, continuous demand.

**Q: Can I compare different fuel types?**
Yes, you can use the `get_efficiency_comparison` tool to see Energy Factor (EF) benchmarks for gas, electric resistance, and heat pump technologies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/water-heater-sizing-calculator](https://vinkius.com/mcp/water-heater-sizing-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Water Heater Sizing Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `water-heater-sizing-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Water Heater Sizing Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "water-heater-sizing-calculator": {
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
