# Reagent Storage & Handling MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/reagent-storage-handling)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design safe reagent storage, pumping, and containment systems.

## Description
This MCP server provides specialized engineering tools for designing reagent storage and handling systems. It enables AI agents to calculate required tank capacity using `get_storage_capacity`, determine necessary pump characteristics with `calculate_pumping_specs`, and ensure safety compliance by using `assess_containment_needs` and `validate_material_compatibility` for hazardous material management.


## Available Tools (4)
- **calculate_pumping_specs**: Determines the necessary pump characteristics to move the reagent
- **get_storage_capacity**: Determines the required storage volume for a specific reagent
- **validate_material_compatibility**: Checks if the proposed storage and pumping hardware is safe for the specific reagent
- **assess_containment_needs**: Calculates the required volume for secondary containment based on hazard levels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reagent Storage & Handling** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much storage capacity do I need for Sulfuric Acid if I use 50 liters a day and get deliveries every 10 days?"

**🤖 AI Agent:**
> You need a total capacity of 500 liters, which includes a 500 liter base capacity for the 10-day interval.

---

**👤 You:**
> "What is the required secondary containment for a 1000L tank containing flammable reagents?"

**🤖 AI Agent:**
> The required secondary containment volume is 1100 liters to meet safety standards for flammable materials.

---

**👤 You:**
> "Is stainless_steel compatible with Nitric Acid?"

**🤖 AI Agent:**
> No, stainless_steel is not recommended for Nitric Acid due to high corrosion risk.


## ❓ FAQ

**Q: How do I calculate the required tank size?**
You can use the `get_storage_capacity` tool by providing the reagent name, daily consumption rate, and the number of days between deliveries.

**Q: Can this tool help with safety compliance?**
Yes, the `assess_containment_needs` tool calculates the required secondary containment volume based on the hazard class of your reagents to ensure regulatory compliance.

**Q: How do I check if a pump is suitable for my reagent?**
Use `calculate_pumping_specs` to find the required head and power, and `validate_material_compatibility` to ensure the pump material is safe for the specific chemical.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/reagent-storage-handling](https://vinkius.com/ai-agent-connect/reagent-storage-handling)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reagent Storage & Handling** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reagent-storage-handling` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reagent Storage & Handling** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reagent-storage-handling": {
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
