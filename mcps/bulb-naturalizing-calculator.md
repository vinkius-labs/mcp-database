# Bulb Naturalizing Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bulb-naturalizing-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate bulb package requirements for naturalized plantings.

## Description
This MCP server provides specialized tools for landscape professionals to plan naturalized bulb plantings. Use `get_required_bulb_count` to determine how many bulbs to purchase by accounting for planting area, desired density, existing inventory, and biological loss rates. You can also use `calculate_package_requirements` to convert bulb counts into commercial package quantities, `get_spacing_from_density` to estimate physical bulb spacing, and `get_area_summary` for a high-level project overview.


## Available Tools (4)
- **calculate_package_requirements**: Converts a raw bulb count into a specific number of commercial packages to purchase
- **get_area_summary**: Provides a high-level overview of the planting project scale
- **get_required_bulb_count**: Calculates the total number of new bulbs needed to meet density goals while accounting for existing inventory and biological loss
- **get_spacing_from_density**: Determines the physical distance between bulbs based on a target density for a specific species


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bulb Naturalizing Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a 500 sq ft area and want a density of 5 bulbs per sq ft. I already have 50 bulbs. With a 10% loss rate, how many bulbs should I buy?"

**🤖 AI Agent:**
> You need to purchase 495 bulbs to meet your density goal after accounting for the 10% loss rate.

---

**👤 You:**
> "How many 50-count bulb packages do I need if I must purchase 230 bulbs?"

**🤖 AI Agent:**
> You need to purchase 5 packages, which will leave you with 20 remaining bulbs.

---

**👤 You:**
> "Give me a summary for a 1000 sq ft project with a density of 10 bulbs per sq ft."

**🤖 AI Agent:**
> The project covers 1000 sq ft with a target of 10,000 total bulbs.


## ❓ FAQ

**Q: How does the tool account for bulb loss?**
The `get_required_bulb_count` tool uses a loss rate parameter to add a buffer for biological attrition like rot or wildlife predation.

**Q: Can I calculate how many bags of bulbs I need to buy?**
Yes, use the `calculate_package_requirements` tool by providing the number of bulbs needed and the size of the commercial package.

**Q: How is bulb spacing determined?**
The `get_spacing_from_density` tool estimates the physical distance between bulbs based on your target density.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bulb-naturalizing-calculator](https://vinkius.com/en/ai-agent-connect/bulb-naturalizing-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bulb Naturalizing Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bulb-naturalizing-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bulb Naturalizing Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bulb-naturalizing-calculator": {
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
