# Sustainable Trip Emissions Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sustainable-trip-emissions-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Calculate the carbon footprint of your travels, including flights, trains, cars, and lodging.

## Description
This MCP server provides precise tools to calculate the environmental impact of travel. Use `get_category_totals` to see a breakdown of emissions by transport, lodging, and food. Use `get_per_person_emissions` to determine individual footprints in group travel, or `compare_scenarios` to evaluate how changing transport modes affects your total impact. For full transparency, `get_factor_assumptions` provides the specific emission factors used in every calculation.


## Available Tools (4)
- **get_category_totals**: Provides a breakdown of total emissions organized by travel and lifestyle categories
- **get_factor_assumptions**: g., "flight", "train", "car").

Retrieves the specific emission factors and logic used for transparency
- **get_per_person_emissions**: Calculates the individual carbon footprint for a group traveling together
- **compare_scenarios**: Compares the current trip configuration against an alternative scenario


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sustainable Trip Emissions Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total emission breakdown for my trip?"

**🤖 AI Agent:**
> Your trip emissions are: Transport: 150kg CO2e, Lodging: 45kg CO2e, Food and Activities: 20kg CO2e. Total: 215kg CO2e.

---

**👤 You:**
> "How much CO2 will each person emit if we travel in a car with 4 people?"

**🤖 AI Agent:**
> With 4 people in the car, the per-person emission is 12.5kg CO2e.

---

**👤 You:**
> "What happens to my emissions if I take a train instead of a flight?"

**🤖 AI Agent:**
> Switching from a flight to a train will reduce your total emissions by 65kg CO2e, a 40% reduction.


## ❓ FAQ

**Q: How are flight emissions calculated?**
Flight emissions are calculated based on distance and cabin class. Higher cabin classes result in higher per-passenger emissions due to increased space and weight allocation.

**Q: Does this tool include carbon offsets?**
No. This tool calculates gross emissions only to maintain scientific integrity and avoid greenwashing.

**Q: Can I compare different travel options?**
Yes, you can use the comparison tool to see the difference in emissions between two different trip configurations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sustainable-trip-emissions-calculator](https://vinkius.com/en/ai-agent-connect/sustainable-trip-emissions-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sustainable Trip Emissions Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sustainable-trip-emissions-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sustainable Trip Emissions Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sustainable-trip-emissions-calculator": {
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
