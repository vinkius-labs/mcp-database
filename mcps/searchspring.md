# Searchspring MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/searchspring)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Empower your AI to search, filter, and recommend e-commerce products using the Searchspring (Athos Commerce) catalog API.

## Description
Connect your **Searchspring** store (now part of Athos Commerce) to any AI agent to interact with your e-commerce product catalog conversationally. Bring enterprise-grade site search and merchandising directly into your AI workflows without manually browsing storefronts.

### What you can do

- **Product Discovery** — Query your catalog using natural language, check stock availability, and pull in high-resolution product images and pricing
- **Merchandising & Filtering** — Narrow down thousands of SKUs using faceted parameters (size, color, brand) or strict price range thresholds instantly
- **Autocomplete Trends** — Expose the exact query suggestions (autocomplete) that your customers are seeing on the front-end to gauge search behavior
- **Catalog Auditing** — Browse through deep category trees or request specific details for a single SKU to verify if product metadata is synced correctly

### How it works

1. Subscribe to this server
2. Enter your unique Searchspring Site ID
3. Start fetching product cards or auditing search logic natively from Claude, Cursor, or any MCP-compatible environment

### Who is this for?

- **E-commerce Managers** — ask the AI to show all out-of-stock items in the 'Mens Shoes' category to identify merchandising gaps
- **Developers** — verify if newly integrated custom JSON facets and sorting rules are being parsed properly by the API before deploying front-end UI changes
- **Customer Support** — quickly lookup an exact SKU to confirm pricing and specs without leaving the chat interface when responding to a customer


## Available Tools
- **search_brand**: Lists products from a specific brand
- **search_category**: g., "Mens>Shoes").

Lists products within a specific category hierarchy
- **search_custom**: Performs a search with custom Searchspring parameters
- **search_filtered**: Format: "key:value,key2:value2".

Performs a filtered product search
- **search_pagination**: Retrieves a specific page of search results
- **search_price_range**: Searches for products within a specific price range
- **search_products**: Searches for products in the Searchspring catalog
- **search_sku**: Retrieves details for a specific product SKU
- **search_sorted**: Format: "key:direction" (e.g., "price:asc").

Performs a sorted product search
- **suggest_queries**: Retrieves autocomplete query suggestions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Searchspring** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search our catalog for 'wireless headphones' and sort the results by price in ascending order."

**🤖 AI Agent:**
> I've fetched the products sorted by price in ascending order. 1. Basic Wireless Buds - $19.99 (In Stock). 2. Studio Sync Headphones - $34.50 (Low Stock). 3. Noise-Canceling Overhead - $49.00. Would you like the thumbnail images attached?

---

**👤 You:**
> "Fetch the product specs and current availability for SKU 'LPTOM-415'."

**🤖 AI Agent:**
> I queried the catalog for SKU LPTOM-415. This correlates to the 'Dell XPS 13 Ultrabook'. Pricing is set at $1,199. It features an i7 processor, 16GB RAM, and 512GB SSD. Current inventory status registers as OUT OF STOCK in our primary warehouse.

---

**👤 You:**
> "Find all products by the brand 'Nike' that cost between $50 and $100."

**🤖 AI Agent:**
> I've pulled the data using `search_brand` combined with `search_price_range`. I found 12 results for Nike between $50 and $100. The top results are: 1. Revolution 6 Running Shoes ($65.00), 2. Sportswear Club Fleece Hoodie ($55.00), and 3. Dri-FIT Training Pants ($70.00).


## ❓ FAQ

**Q: Can the AI filter catalog products by specific colors or variations?**
Yes. You can instruct the agent: 'Find all Men's Shirts and filter by color: Blue and size: Medium'. The agent will natively invoke `search_filtered` passing the specific parameter facets to narrow down exactly what is requested.

**Q: Can I check autocomplete queries directly from the chat prompt?**
Absolutely. Use the prompt: 'What queries do you suggest when someone types "runn"?'. The agent fires `suggest_queries` simulating a shopper and returns search trends such as 'running shoes', 'running shorts', demonstrating what customers see.

**Q: How do I ensure the integration only searches within a specific category?**
You can explicitly ask the AI to restrict the search. For example: 'Using the Searchspring API, list the top 5 products strictly in the Electronics > Audio category'. The agent invokes `search_category`, returning items isolated within that structural path.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/searchspring](https://vinkius.com/mcp/searchspring)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Searchspring** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `searchspring` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Searchspring** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "searchspring": {
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
