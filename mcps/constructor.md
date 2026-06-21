# Constructor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/constructor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Empower e-commerce discovery via Constructor.io — perform ML-ranked product searches, get personalized recommendations, and audit browse categories directly from any AI agent.

## Description
Connect your **Constructor.io** account to any AI agent and take full control of your site search and product discovery workflows through natural conversation.

### What you can do

- **AI-Powered Search** — Execute ML-ranked product retrieval dynamically mapped to e-commerce signals and user intent
- **Predictive Autocomplete** — Access fast predictive typing boundaries and trace exact matched categories for any partial query
- **Dynamic Recommendations** — Surface personalized products using collaborative filtering models and custom recommendation pods
- **Category & Brand Browsing** — Navigate through product directory trees and manufacturer taxonomies without any query bias
- **Advanced Filtering** — Apply strict attribute filters (colors, sizes, features) and custom sort rules to refine product discovery results
- **Collection Management** — Retrieve curated marketing clusters and static collections accurately for promotional auditing

### How it works

1. Subscribe to this server
2. Enter your Constructor.io Public API Key (found in Dashboard > Integration)
3. Start optimizing your e-commerce discovery from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — audit search rankings and recommendation pods without manual dashboard testing
- **Product Owners** — monitor category browsing performance and verify attribute filtering logic in real-time
- **Developers** — test and debug search API parameters and personalized recommendation outputs through natural language
- **Marketing Teams** — verify that curated collections and brand taxonomies are correctly mapped and rankable


## Available Tools
- **autocomplete**: Perform structural extraction of properties driving active Account logic
- **browse_brand**: Inspect deep internal arrays mitigating specific Plan Math
- **browse_category**: Provision a highly-available JSON Payload generating hard Customer bindings
- **browse_collection**: Identify precise active arrays spanning native Gateway auth
- **custom_search**: Identify precise active arrays spanning native Hold parsing
- **search_filtered**: ]` bounding JSON structures restricting arrays to exact colors/sizes or features.

Irreversibly vaporize explicit validations extracting rich Churn flags
- **search_pagination**: Dispatch an automated validation check routing explicit Gateway history
- **get_recommendations**: Retrieve explicit Cloud logging tracing explicit Vault limits
- **search_products**: Identify bounded CRM records inside the Headless Constructor.io Platform
- **search_sorted**: Enumerate explicitly attached structured rules exporting active Billing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Constructor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'running shoes' in Constructor"

**🤖 AI Agent:**
> Searching for 'running shoes'... I found 120 products. The top ML-ranked items are 'Ultra-Light Runner' ($120) and 'Trail Master v2' ($145). Would you like to apply any filters like size or brand?

---

**👤 You:**
> "What products are recommended in the 'home-page-trending' pod?"

**🤖 AI Agent:**
> Retrieving trending recommendations... I found 5 items including 'Eco-Friendly Yoga Mat' and 'Wireless Noise-Cancelling Headphones'. These are currently trending based on your global collaborative filtering model.

---

**👤 You:**
> "Browse the 'Outdoor Furniture' category"

**🤖 AI Agent:**
> Browsing 'Outdoor Furniture' (ID: group_789)... I found 45 products in this category hierarchy. Top sub-categories include 'Patio Sets' and 'Garden Chairs'.


## ❓ FAQ

**Q: Can my agent check the ML ranking for a specific product search?**
Yes. Use the 'search_products' tool. The agent will retrieve results ranked by Constructor's ML engine, allowing you to audit how products are surfaced based on specific keywords and intent signals.

**Q: How do I retrieve personalized recommendations via the agent?**
Provide the 'pod_id' to your agent and use the 'get_recommendations' tool. The agent will query the collaborative filtering models to return a list of products tailored to your specified recommendation logic.

**Q: Can I test attribute filtering like color or size through chat?**
Absolutely. The 'search_filtered' tool allows you to pass exact attribute mappings (e.g., 'color:blue,size:L'). Your agent will verify how the API restricts results to those specific structural bounds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/constructor](https://vinkius.com/mcp/constructor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Constructor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `constructor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Constructor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "constructor": {
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
