# USDA FoodData Central MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/usda-fooddata-central-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Manage your nutritional research — audit food records and nutrient data via AI.

## Description
Empower your AI agent to orchestrate your entire nutritional research workflow with **USDA FoodData Central**, the authoritative source for food composition data. By connecting USDA FoodData to your agent, you transform complex nutrient searches into a natural conversation. Your agent can instantly search for food items, audit nutritional metadata, and retrieve detailed composition reports without you ever touching a technical database. Whether you are building a diet plan or conducting food science research, your agent acts as a real-time nutritionist, ensuring your data is always accurate and comprehensive.

### What you can do

- **Food Auditing** — Search for thousands of food items by keyword and retrieve detailed metadata, including FDC IDs and brand names.
- **Nutrient Oversight** — Retrieve full nutrient profiles for specific foods to maintain a clear view of caloric and mineral content.
- **Batch Discovery** — List multiple food items simultaneously to compare nutritional values across different categories.
- **Composition Intelligence** — Query specialized survey data and foundation records to maintain strict control over food science research.
- **Metadata Discovery** — List all available nutrients in the USDA catalog to identify specific dietary markers.

### How it works

1. Subscribe to this server
2. Enter your USDA API Key
3. Start managing your nutritional intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Nutritionists & Dietitians** — monitor food composition and nutrient values straight from your workflow.
- **Food Scientists** — verify detailed mineral and vitamin profiles without manual database exports.
- **Health Enthusiasts** — perform rapid audits of food items and discover nutritional breakdowns through natural language.
- **App Developers** — automate food data querying to orchestrate your health-tech projects smoothly.




## 💬 Prompt Examples

Here are some examples of how you can interact with the **USDA FoodData Central** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'greek yogurt' in the USDA database."

**🤖 AI Agent:**
> I've retrieved several entries for greek yogurt. Notable options include low-fat and whole milk versions. Would you like the nutrient details for any specific brand?

---

**👤 You:**
> "Show nutritional details for FDC ID 170895."

**🤖 AI Agent:**
> I've identified FDC ID 170895 as 'Raw Spinach'. It contains high levels of Vitamin A and K. Would you like the full breakdown per 100g?

---

**👤 You:**
> "List available nutrients in the USDA catalog."

**🤖 AI Agent:**
> I've scanned the nutrient catalog. It includes over 200 items, from 'Energy' and 'Protein' to specific minerals like 'Selenium'. I can help you search for a specific dietary marker.


## ❓ FAQ

**Q: How do I find my USDA API Key?**
Sign up at the [**USDA API portal**](https://api.nal.usda.gov/), and you will receive your API Key via email. Copy and paste it below.

**Q: Can the agent search for branded food items?**
Yes. Use the `search_foods` tool and set the `dataType` to 'Branded'. Your agent will retrieve specific products from various manufacturers instantly.

**Q: Is it possible to retrieve a full nutritional breakdown?**
Yes. The `get_food` tool provides a comprehensive list of nutrients, including vitamins, minerals, and caloric data for any specific FDC ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/usda-fooddata-central-alternative](https://vinkius.com/mcp/usda-fooddata-central-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **USDA FoodData Central** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `usda-fooddata-central-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **USDA FoodData Central** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "usda-fooddata-central-alternative": {
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
