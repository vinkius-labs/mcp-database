# Animal Feed Formulator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/animal-feed-formulator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Optimizes cost-effective animal diets using linear programming.

## Description
This MCP server provides an optimization engine for animal nutrition. It uses the simplex method to calculate the most cost-effective ingredient combinations that satisfy specific nutritional profiles for cattle, swine, and poultry. Users can retrieve species-specific requirements using `get_species_requirements`, browse available ingredients with `get_available_ingredients`, and generate optimal diets via `formulate_ration`. The server also includes `validate_ration_safety` to ensure formulated mixes stay within biological safety thresholds.


## Available Tools (4)
- **get_species_requirements**: Retrieves the standard nutritional target ranges for a specific animal species
- **get_available_ingredients**: Lists all ingredients available for formulation, including their nutritional content and cost
- **validate_ration_safety**: Checks if a previously formulated ration complies with safety thresholds for specific nutrients
- **formulate_ration**: Executes the linear programming optimization to create the cheapest possible feed mix


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Animal Feed Formulator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the nutritional requirements for cattle?"

**🤖 AI Agent:**
> Cattle require specific ranges for Crude Protein, TDN, and NDF to maintain health and growth.

---

**👤 You:**
> "Formulate a ration for 500kg of swine feed."

**🤖 AI Agent:**
> The optimized ration for 500kg of swine feed consists of 60% corn and 40% soybean meal, with a total cost of $125.00.

---

**👤 You:**
> "Is this ration safe for poultry: 70% corn and 30% soybean meal?"

**🤖 AI Agent:**
> The ration is valid and meets the safety thresholds for poultry.


## ❓ FAQ

**Q: What species are supported?**
The engine currently supports nutritional profiles for cattle, swine, and poultry.

**Q: How does the optimization work?**
It uses the simplex method (linear programming) to minimize the total cost of the ration while meeting all minimum and maximum nutrient constraints.

**Q: Can I set custom nutrient limits?**
Yes, you can provide custom constraints during the `formulate_ration` process to override standard species requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/animal-feed-formulator](https://vinkius.com/ai-agent-connect/animal-feed-formulator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Animal Feed Formulator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `animal-feed-formulator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Animal Feed Formulator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "animal-feed-formulator": {
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
