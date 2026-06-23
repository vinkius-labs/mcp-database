# Cocktail API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cocktail-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search cocktail recipes — audit ingredients and instructions via AI.

## Description
Empower your AI agent to orchestrate your entire mixology research and recipe auditing workflow with the **Cocktail API**, the comprehensive source for global drink data. By connecting the API Ninjas Cocktail API to your agent, you transform complex recipe searches into a natural conversation. Your agent can instantly retrieve cocktail details, audit ingredient lists, and query preparation instructions without you ever touching a drink portal. Whether you are planning a menu or conducting regional mixology research, your agent acts as a real-time sommelier, ensuring your data is always precise and localized.

### What you can do

- **Recipe Auditing** — Search for thousands of cocktail recipes by name and retrieve detailed metadata, including ingredient lists and instructions.
- **Ingredient Oversight** — Find cocktails matching specific ingredients to understand the thematic distribution of flavors instantly.
- **Discovery by Theme** — Query recipes containing base spirits like 'vodka' or 'tequila' to identify relevant assets for your menu.
- **Preparation Intelligence** — Retrieve full step-by-step instructions for any cocktail to assist in deep-dive mixology classification.
- **Classic Variations** — Instantly retrieve classic iterations of standard beverages, from margaritas to martinis.

### How it works

1. Subscribe to this server
2. Enter your API Ninjas API Key
3. Start managing your mixology intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Bartenders & Mixologists** — monitor recipe data and retrieve ingredient metadata straight from your workflow.
- **Hospitality Leads** — verify drink availability and audit menu distributions without manual searching.
- **Enthusiasts** — perform rapid audits of cocktail recipes and identify relevant drink markers through natural language.
- **Operations Leads** — automate recipe data querying to orchestrate cross-functional hospitality teams smoothly.


## Available Tools (8)
- **get_cocktails_by_ingredients**: Find cocktail recipes by specific ingredients
- **get_classic_margaritas**: Get classic Margarita variations
- **get_classic_martinis**: Get classic Martini variations
- **get_gin_cocktails**: Get popular Gin cocktails
- **get_rum_cocktails**: Get popular Rum cocktails
- **get_tequila_cocktails**: Get popular Tequila cocktails
- **get_vodka_cocktails**: Get popular Vodka cocktails
- **search_cocktails**: Search for cocktail recipes by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cocktail API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the recipe for a 'Margarita' using Cocktail API."

**🤖 AI Agent:**
> I've retrieved the recipe for a Margarita! It includes tequila, triple sec, and lime juice. The instructions specify shaking the ingredients with ice and serving in a salt-rimmed glass. Would you like to see similar tequila-based cocktails?

---

**👤 You:**
> "Find cocktails that contain 'vodka' and 'coffee'."

**🤖 AI Agent:**
> I've identified several cocktails matching your ingredients! The primary match is the 'Espresso Martini'. I can provide the full ingredient list and instructions for this drink if you'd like.

---

**👤 You:**
> "Show recipes for 'Gin and Tonic'."

**🤖 AI Agent:**
> I've retrieved the details for Gin and Tonic. It typically contains gin and tonic water, garnished with a lime wedge. I can assist you with more variation metadata if needed.


## ❓ FAQ

**Q: How do I find my API Ninjas Key?**
Log in to your [**API Ninjas dashboard**](https://api-ninjas.com/profile), and you will find your API Key on the main page. Copy and paste it below.

**Q: Can I search for cocktails by ingredients?**
Yes. Use the `get_cocktails_by_ingredients` tool providing a comma-separated list (e.g., 'vodka,orange juice'). Your agent will return matching recipes instantly.

**Q: Does it support detailed instructions?**
Yes. Every cocktail recipe retrieved by your agent includes the official preparation instructions provided by API Ninjas.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cocktail-api](https://vinkius.com/mcp/cocktail-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cocktail API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cocktail-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cocktail API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cocktail-api": {
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
