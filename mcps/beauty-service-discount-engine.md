# Beauty Service Discount Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/beauty-service-discount-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates discounted service prices for beauty salons using loyalty and seasonal rules.

## Description
This MCP server provides a specialized pricing engine for beauty salon services. It connects AI agents to salon operations by calculating final costs based on customer loyalty tiers, service categories, and active seasonal promotions. Use `get_service_base_price` to find standard costs, `get_customer_loyalty_discount` to check customer status, and `calculate_final_service_price` to determine the total amount a customer should pay after all applicable discounts are applied.


## Available Tools (4)
- **calculate_final_service_price**: Calculates the final amount the customer must pay by aggregating all applicable discounts
- **calculate_seasonal_promotion**: Checks if a specific service qualifies for an active seasonal or event-based promotion
- **get_customer_loyalty_discount**: Determines the discount percentage available to a customer based on their loyalty status
- **get_service_base_price**: Retrieves the standard cost of a specific beauty service


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beauty Service Discount Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the final price for customer C123 for a haircut (service S456) today?"

**🤖 AI Agent:**
> The final price for the haircut is $45.00, with a total savings of $15.00 applied.

---

**👤 You:**
> "How much does a manicure cost normally?"

**🤖 AI Agent:**
> The standard base price for a manicure is $35.00.

---

**👤 You:**
> "Check if there are any seasonal promotions for service S789 on 2024-12-25."

**🤖 AI Agent:**
> Yes, there is a Holiday Special promotion active for this service with a 15% discount.


## ❓ FAQ

**Q: How are discounts applied?**
Discounts are applied sequentially. The loyalty discount and seasonal promotion rates are compounded to reach the final price.

**Q: Can I check the base price of a service?**
Yes, you can use the `get_service_base_price` tool to retrieve the standard cost of any service in the catalog.

**Q: Is there a limit on how much a discount can be?**
Yes, all calculations respect a global maximum discount cap and a minimum margin threshold for each service category.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/beauty-service-discount-engine](https://vinkius.com/en/ai-agent-connect/beauty-service-discount-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Beauty Service Discount Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `beauty-service-discount-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Beauty Service Discount Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "beauty-service-discount-engine": {
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
