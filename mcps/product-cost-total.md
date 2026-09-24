# Product Cost Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/product-cost-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Aggregate and audit cumulative costs for product components and inventory.

## Description
This MCP server provides tools to manage and audit product manufacturing costs. It allows for retrieving individual component prices via `get_component_cost`, calculating the full cost of a product using `calculate_product_total`, summing costs for specific value tiers with `aggregate_category_costs`, and performing budget audits with `audit_cost_discrepancy`.


## Available Tools (4)
- **aggregate_category_costs**: Sums the total costs of all products belonging to a specific value tier
- **audit_cost_discrepancy**: Compares a calculated product cost against a provided reference value to identify overruns or underruns
- **calculate_product_total**: Calculates the full cost of a single product based on its constituent parts
- **get_component_cost**: Retrieves the base cost of a specific component


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Product Cost Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost for product P-100 if it uses 2 units of component C-01 and 1 unit of component C-02?"

**🤖 AI Agent:**
> The total cost for product P-100 is $150.00.

---

**👤 You:**
> "Check if the cost for product P-500 matches my budget of $500."

**🤖 AI Agent:**
> The product P-500 cost is $510.00, which is $10.00 over your expected budget.

---

**👤 You:**
> "How much is the total value of all products in the High-Value tier?"

**🤖 AI Agent:**
> The total value for the High-Value tier is $12,450.00 across 15 products.


## ❓ FAQ

**Q: How do I calculate the total cost of a product?**
You can use the `calculate_product_total` tool by providing the product ID and a map of the component quantities used.

**Q: Can I audit my product costs against a budget?**
Yes, the `audit_cost_discrepancy` tool compares the calculated cost against your expected budget to identify differences.

**Q: How can I see the total value of a specific cost tier?**
Use the `aggregate_category_costs` tool to get the total value and product count for tiers like Low-Value, Mid-Value, or High-Value.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/product-cost-total](https://vinkius.com/en/ai-agent-connect/product-cost-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Product Cost Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `product-cost-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Product Cost Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "product-cost-total": {
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
