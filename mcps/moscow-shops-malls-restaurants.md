# Moscow Shops, Malls & Restaurants MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moscow-shops-malls-restaurants)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [food-beverage](../categories/food-beverage.md)

Keyless Moscow retail and food: shops by class (28 types), malls, markets, restaurants and cafes, citywide category counts and top shop chains.

## Description
Where to buy or eat in Moscow, keyless, from OpenStreetMap — about 6,600 supermarkets, 3,500 restaurants, 6,200 fast-food outlets and 7,200 cafes inside the city.

### What you can do
- **find_shops** — shops of one class (28 types: supermarket, convenience, electronics, clothes, pharmacy-like chemist and more), filterable by brand, open now and proximity
- **find_malls** — shopping centres (about 120), from Aviapark to Vavilon, filterable by name and proximity
- **find_markets** — food and street markets (about 80), e.g. Danilovsky, filterable by name and open now
- **find_restaurants** — restaurants, fast food and cafes (any or one kind), filterable by cuisine fragment, open now and proximity
- **shopping_category_counts** — one call with citywide counts for nine retail and food classes
- **top_shop_brands** — the retail chains the map records most often (a 500-shop sample), ranked — use it to discover the exact brand values before find_shops

### Who is this for
Anyone shopping or eating in Moscow: finding the nearest supermarket, a mall, a late dinner, or an app that ranks the city’s retail chains.


## Available Tools (6)
- **find_malls**: Each row carries the name (e.g. "Авиапарк", "Золотой Вавилон РИО"), the operator, the shop count tag and the centre coordinate. Filter by name fragment or by proximity to a point.

Find shopping centres in Moscow
- **find_markets**: g. "Даниловский рынок", "Усачёвский рынок", "Рижский рынок"). Each row carries the name, operator, opening hours and the centre coordinate. Filter by name fragment, open_now or proximity to a point.

Find markets in Moscow
- **find_restaurants**: Pass kind to choose: "restaurant" (default), "fast_food", "cafe" or "any" (all three). Filter by cuisine fragment (e.g. "русской", "italian", "грузинская", "sushi", "coffee_shop" — values are as mapped, mixed Russian/English) and by open_now. Each row carries the name, cuisine, phone, opening hours and outdoor-seating/delivery flags.

Find restaurants and cafes in Moscow
- **find_shops**: Pass type to choose the shop class: "supermarket" (default), "convenience", "department_store", "mall", "bakery", "greengrocer", "dairy", "butcher", "seafood", "confectionery", "alcohol", "beverages", "electronics", "mobile_phone", "clothes", "shoes", "cosmetics", "chemist", "books", "stationery", "toys", "jewellery", "optician", "furniture", "hardware", "garden_centre" or "pet". Each row carries the name, brand, phone and opening hours; open_now: "true" keeps only shops open at the moment of the call.

Find shops in Moscow
- **shopping_category_counts**: Use it to size a category before listing it with find_shops or find_restaurants.

Count shops and food places across Moscow
- **top_shop_brands**: g. "Пятёрочка", "Магнит", "ВкусВилл", "DNS", "Ситилинк". Use it before find_shops to discover the exact brand values a chain is mapped under. The ranking reflects a 500-row sample of the mapped shops, not the whole market.

Rank shop chains by mapped presence in Moscow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moscow Shops, Malls & Restaurants** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find a supermarket open now near the centre."

**🤖 AI Agent:**
> find_shops with type: "supermarket", open_now: "true" and the centre coordinates lists them by proximity with hours and phone.

---

**👤 You:**
> "Which grocery chains dominate Moscow?"

**🤖 AI Agent:**
> top_shop_brands ranks the chains by mapped presence (a 500-shop sample); use the exact brand value with find_shops to list their stores.

---

**👤 You:**
> "Where can I eat Georgian food nearby?"

**🤖 AI Agent:**
> find_restaurants with kind: "any", cuisine: "грузинская" (or "georgian") and your lat/lon lists the matches with cuisine, hours and delivery flags.


## ❓ FAQ

**Q: Do I need an API key?**
No. Every source is keyless and global: OpenStreetMap (Overpass + Nominatim), Open-Meteo and Russian Wikipedia. The MCP defines no credentials.

**Q: Why does a chain appear more than once under different names?**
The map records brand tags as mappers wrote them (Пятёрочка, Pyaterochka, 5ka). top_shop_brands shows the variants ranked by frequency — pick the exact value for find_shops.

**Q: Why are the counts bigger than the listed rows?**
Yes. OSM maps most large venues as areas (buildings, park outlines), and every tool uses the nwr selector, so nodes, ways and relations all count. Point-only queries would miss them.

**Q: Can I find shops near me?**
Pass lat + lon (and optionally km, 0.1–25) and the query narrows to a radius instead of the whole city. Use it before a long list — a citywide scan is heavy and capped at 200 rows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moscow-shops-malls-restaurants](https://vinkius.com/en/ai-agent-connect/moscow-shops-malls-restaurants)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moscow Shops, Malls & Restaurants** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moscow-shops-malls-restaurants` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moscow Shops, Malls & Restaurants** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moscow-shops-malls-restaurants": {
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
