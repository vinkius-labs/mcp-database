# Preço do Gás MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/preco-do-gas)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [energy-utilities](../categories/energy-utilities.md)

Look up the current cooking-gas price near any Brazilian address or CEP: how much a botijão costs, who delivers it and in how long — from the resellers of Preço do Gás, the largest gas reseller network in Brazil.

## Description
Preço do Gás (precodogas.com.br) is the largest gas reseller network in Brazil, connecting consumers to brands like Supergasbrás, Ultragaz and Liquigás that deliver to their exact address. This MCP server exposes that network to AI agents. Given only a Brazilian address, `search_gas_prices` geocodes the location internally using free keyless providers (OpenStreetMap Nominatim with ArcGIS World Geocoder as failback), then queries the reseller API to return a timestamped snapshot: brands, prices, discounts, delivery windows, ratings, open status, opening hours, accepted payment methods, and editorialed highlights (cheapest, fastest delivery, top rated). `lookup_cep` resolves a postal code through the provider's own address index — the same coordinates that define delivery coverage. `list_gas_products` enumerates the products that can be filtered on (13kg cooking gas, 45kg commercial cylinders, 20kg forklift cylinders, water gallons, etc.), `track_gas_order` looks up whether an order was registered for a Brazilian phone number, and `list_gas_news` streams articles from the official Preço do Gás blog (gas prices, delivery regions, Vale Gás, safety, brands) with category filtering. Gas prices genuinely vary by neighbourhood, brand, payment method and active campaigns, so every snapshot carries the time it was taken and a note explaining that. No credentials are required: the backend token is obtained from the site's public /jwt.php endpoint on every call. Every response carries a ready-to-quote `answer` field — an executive summary in pt-BR that agents can read or relay as-is — and price searches additionally include `priceStats` (lowest, highest and average price across all matching resellers, plus how many are open now). Tool routing: gas price at an address/CEP → `search_gas_prices`; gas news → `list_gas_news`; product codes → `list_gas_products`; CEP coverage → `lookup_cep`; order status → `track_gas_order`.


## Available Tools (5)
- **list_gas_products**: If the user just wants the price, skip it and call search_gas_prices directly.

Lists the gas product codes a price search accepts (gás 13kg, comercial 45kg, água 20kg, etc.). Catalog only — it does not return prices; for the price, use search_gas_prices
- **list_gas_news**: Never for price questions ("qual o preço do gás?" → search_gas_prices). Category is optional, accents-insensitive; valid: Preço do gás, Revendas de gás, Regiões de entrega, Vale gás, Gás de cozinha, Botijão de Gás, Comprar gás, Segurança, Marcas, GLP, Economia, Aquecedor à gás, Aplicativo, Notícias, Receitas, Dicas de casa, Geral.

Fetches articles from the official Preço do Gás blog (gas news, Vale Gás, campaigns, safety). Blog content — it does NOT return current prices; for the gas price use search_gas_prices
- **lookup_cep**: When the user wants the price at a CEP, call search_gas_prices (it geocodes CEPs internally).

Resolves a CEP to street, neighbourhood, city, UF and whether the area has gas delivery coverage. Not a price lookup — for the price at a CEP, use search_gas_prices
- **track_gas_order**: Phone: DDD + number in any format ((11) 99999-8888, +55 11 99999-8888, 5511999998888). Not for prices (search_gas_prices) or news (list_gas_news).

Tracks a gas order by the phone number it was placed with ("onde está meu pedido de gás?"). Returns status, tracking token and detail link. Not a price lookup
- **search_gas_prices**: A CEP alone is a valid location — pass it in `address` or in `cep` (e.g. "22041-020"). Do NOT use for news (list_gas_news), order tracking (track_gas_order) or CEP coverage checks (lookup_cep).

Looks up the current cooking-gas price for a location in Brazil — the answer to "how much is gas?", "qual o preço do gás?" and "quanto custa o botijão?". Pass the location as `address` (street, city or CEP) and/or `cep` (postal code alone). Returns resellers that deliver there ranked by price (cheapest first by default), market stats and a ready-to-read pt-BR answer. Each result carries a `url` (that reseller's direct order link); the search also carries `priceListUrl` (page listing all prices for the location). Fetch only if more detail is needed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Preço do Gás** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much does a 13kg cooking gas cost near Rua Augusta 500, São Paulo - SP?"

**🤖 AI Agent:**
> The cheapest reseller delivering to Rua Augusta 500 offers Gás de Cozinha 13kg at R$ 116.90 (Supergasbrás, delivery in 60-90 min, open now). 3 more options are available from R$ 117.99. Snapshot taken 14:32 — prices vary by time and campaign.

---

**👤 You:**
> "Find the fastest gas delivery at CEP 30110-000 (Belo Horizonte) and show the top rated resellers."

**🤖 AI Agent:**
> For CEP 30110-000 the fastest option is a reseller delivering in 10-40 minutes; sorted by rating, Servgás (4.7) and Ultragaz (4.7) lead.

---

**👤 You:**
> "Track my gas order placed with phone 11987654321."

**🤖 AI Agent:**
> An order is registered for 11987654321. You can open its details at the returned order link.


## ❓ FAQ

**Q: How do I check the gas price near my address?**
Use `search_gas_prices` with your address, e.g. "Avenida Paulista 1000, São Paulo - SP". The tool geocodes the address itself (no coordinates needed) and returns resellers sorted by lowest price by default, with highlights for the cheapest, fastest and top-rated options. The response includes a ready-to-read `answer` summary plus `priceStats` (min/max/average and how many resellers are open now).

**Q: Do I need an API key or credentials?**
No. The reseller API authenticates with a public JWT served by the site's own /jwt.php endpoint, refreshed automatically on each call. Geocoding uses free, keyless providers with failback (Nominatim → ArcGIS → bare CEP).

**Q: Are the prices fixed?**
No — gas prices vary by neighbourhood, brand, product, payment method and active campaigns, and change over time. Each `search_gas_prices` call returns a timestamped snapshot with a note about that variability.

**Q: Can I track an order I placed through the app?**
Yes. `track_gas_order` accepts the Brazilian phone number (DDD + number) used to place the order and reports whether it is registered, with the detail-page link when it is.

**Q: Does a CEP have gas delivery coverage?**
Use `lookup_cep` with the postal code. It answers from the provider's own address index (the coordinates used to define delivery areas), returning street, neighbourhood, city and UF. If found, running `search_gas_prices` on that CEP shows the live resellers that serve it.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/preco-do-gas](https://vinkius.com/en/ai-agent-connect/preco-do-gas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Preço do Gás** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `preco-do-gas` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Preço do Gás** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "preco-do-gas": {
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
