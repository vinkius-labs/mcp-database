# Shaking Table Design Engineer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/shaking-table-design-engineer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculates physical parameters and capacity requirements for mineral processing shaking tables.

## Description
This MCP server provides specialized engineering tools for designing gravity separation systems. It allows AI agents to calculate precise table dimensions using `get_single_table_specs`, determine fleet arrangements with `calculate_fleet_requirements`, optimize deck layouts via `design_deck_configuration`, and establish necessary wash water volumes through `water_requirement_calc`. It is designed for mineral processing engineers to automate capacity and configuration planning.


## Available Tools (4)
- **calculate_fleet_requirements**: Determines how many tables are needed to meet the total feed rate and how they should be arranged
- **design_deck_configuration**: Determines the physical setup of the decks, including width and length ratios, to optimize particle travel
- **get_single_table_specs**: Calculates the required dimensions and area for a single shaking table based on the target feed rate
- **water_requirement_calc**: Calculates the necessary wash water flow rate to maintain proper separation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shaking Table Design Engineer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the dimensions for a single table processing 5 tonnes per hour with a mineral density of 3.5 and feed density of 2.5?"

**🤖 AI Agent:**
> The required table will have a deck length of 2.5m and a deck width of 1.2m, providing a total deck area of 3.0m².

---

**👤 You:**
> "How many tables do I need for a 20 tph feed if each table has an area of 2.5m² in a parallel configuration?"

**🤖 AI Agent:**
> You will need 8 tables arranged in a parallel configuration to meet the 20 tph feed rate.

---

**👤 You:**
> "Calculate the wash water needed for 10 tph feed, mineral density 4.0, and a water-to-feed ratio of 2.0."

**🤖 AI Agent:**
> The required wash water flow rate is 20.0 m³/h.


## ❓ FAQ

**Q: How do I calculate the number of tables needed for my operation?**
You can use the `calculate_fleet_requirements` tool by providing the total feed rate, the area of a single unit, and your preferred configuration (parallel or series).

**Q: Can I design specific deck dimensions?**
Yes, the `design_deck_configuration` tool allows you to specify the number of tables, desired width, and aspect ratio to optimize particle travel.

**Q: How is wash water volume determined?**
The `water_requirement_calc` tool calculates the necessary flow rate based on the feed rate, mineral density, and the specified water-to-feed ratio.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/shaking-table-design-engineer](https://vinkius.com/en/ai-agent-connect/shaking-table-design-engineer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shaking Table Design Engineer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shaking-table-design-engineer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shaking Table Design Engineer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shaking-table-design-engineer": {
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
