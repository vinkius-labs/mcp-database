# ReciPal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/recipal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Manage food recipes — audit ingredients and nutrition via AI.

## Description
Empower your AI agent to orchestrate your entire food manufacturing and recipe auditing workflow with **ReciPal**, the specialized source for nutritional labeling data. By connecting ReciPal to your agent, you transform complex ingredient analysis into a natural conversation. Your agent can instantly retrieve recipe details, audit calorie counts, and query ingredient lists without you ever touching a labeling portal. Whether you are conducting product research or managing regional dietary constraints, your agent acts as a real-time nutritional consultant, ensuring your data is always verified and precise.

### What you can do

- **Recipe Auditing** — Retrieve high-resolution details for all recipes in your catalog, including names, calorie counts, and serving metadata.
- **Ingredient Oversight** — Audit the available ingredients in the ReciPal database to understand the thematic distribution of components instantly.
- **Nutritional Intelligence** — Query full nutritional breakdowns for specific recipes to assist in deep-dive dietary classification.
- **Resource Discovery** — Retrieve unique recipe identifiers to help you identify relevant markers for your food products.
- **Operational Monitoring** — Check API status to ensure your nutritional research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your ReciPal API Key
3. Start managing your nutritional intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Food Manufacturers** — monitor recipe compliance and retrieve nutritional metadata straight from your workflow.
- **Chefs & Nutritionists** — verify ingredient breakdowns and audit calorie counts without manual searching.
- **Compliance Leads** — perform rapid audits of labeling markers and identify relevant dietary patterns through natural language.
- **Operations Leads** — automate food data querying to orchestrate cross-functional manufacturing teams smoothly.


## Available Tools (4)
- **check_api_status**: Check if the ReciPal service is operational
- **get_recipe_details**: Get full nutritional and ingredient details for a specific recipe by ID
- **list_recipal_ingredients**: List all ingredients available in the ReciPal database
- **list_recipal_recipes**: List all recipes in your ReciPal account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ReciPal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my recipes using ReciPal."

**🤖 AI Agent:**
> I've retrieved your recipe catalog! You have several items, including 'Signature Granola' and 'Organic Protein Bar'. Would you like the nutritional details or serving metadata for any of these?

---

**👤 You:**
> "What are the details for recipe ID '12345'?"

**🤖 AI Agent:**
> I've retrieved the details for recipe 12345! It has 250 calories per serving and includes ingredients such as oats and honey. I can provide the full nutritional breakdown or serving counts for you.

---

**👤 You:**
> "List all ingredients available in ReciPal."

**🤖 AI Agent:**
> I've scanned the ingredient catalog from ReciPal! There are thousands of items listed, from common grains to specialized additives. I can assist you with a search to identify the exact markers for your recipe.


## ❓ FAQ

**Q: How do I find my ReciPal API Key?**
Log in to your [**ReciPal account**](https://recipal.com/), navigate to your account settings, and you will find your API Key in the integrations or developer section. Copy and paste it below.

**Q: Can the agent show serving sizes?**
Yes. Every recipe record retrieved by your agent includes serving size metadata and the number of servings per recipe.

**Q: Does it support ingredient lists?**
Yes. The `get_recipe_details` tool retrieves the full list of ingredients used in a specific recipe, along with their weights.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/recipal](https://vinkius.com/mcp/recipal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ReciPal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `recipal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ReciPal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recipal": {
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
