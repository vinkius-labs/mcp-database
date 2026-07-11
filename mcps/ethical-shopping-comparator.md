# Ethical Shopping Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ethical-shopping-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Compare products based on sustainability metrics like carbon footprint, repairability, and durability.

## Description
The Ethical Shopping Comparator allows AI agents to evaluate product sustainability by calculating environmental impact, cost-per-use, and long-term value. Using tools like `calculate_product_metrics`, users can determine the true ecological cost of a purchase. The server also provides `rank_products_by_sustainability` for comparing multiple items and `get_category_benchmarks` to see industry standards.


## Available Tools (3)
- **get_category_benchmarks**: g., Apparel, Electronics, Home Goods).

Retrieves standard sustainability thresholds for a particular product category
- **calculate_product_metrics**: Analyzes a single product to determine its economic and environmental efficiency metrics
- **rank_products_by_sustainability**: Ranks products based on a weighted composite score


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ethical Shopping Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate metrics for a $100 jacket with a durability of 5 years and usage of 20 times per year."

**🤖 AI Agent:**
> The cost-per-use is $1.00, and the estimated true cost including environmental externalities is $115.00.

---

**👤 You:**
> "Which is better for the environment: a durable cotton shirt or a cheap polyester one?"

**🤖 AI Agent:**
> The durable cotton shirt ranks higher because its superior durability score and lower carbon footprint result in a better sustainability score.

---

**👤 You:**
> "What is the repairability threshold for Apparel?"

**🤖 AI Agent:**
> The minimum repairability index threshold for the Apparel category is 6.


## ❓ FAQ

**Q: How can I calculate the environmental impact of a single item?**
Use the `calculate_product_metrics` tool with your product data to find the cost-per-use and true cost.

**Q: Can I compare multiple products at once?**
Yes, use the `rank_products_by_sustainability` tool to rank a list of products based on your preferred weighting (environment, economy, or ethics).

**Q: How do I know if a product meets industry standards?**
You can retrieve standard thresholds for categories like Electronics or Apparel using the `get_category_benchmarks` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ethical-shopping-comparator](https://vinkius.com/mcp/ethical-shopping-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ethical Shopping Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ethical-shopping-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ethical Shopping Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ethical-shopping-comparator": {
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
