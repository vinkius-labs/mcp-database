# Salon Service Pricing Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/salon-service-pricing-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise service pricing, profit margins, and professional earnings for salon services.

## Description
This MCP server provides a complete financial toolkit for salon owners and professionals. It bridges the gap between raw service costs and final customer pricing. Use `generate_pricing_summary` to get a full breakdown of costs, recommended prices, and professional net earnings in one step. You can also use `get_cost_breakdown` to isolate internal costs, `calculate_price_options` to model different tax and margin scenarios, or `calculate_provider_net` to determine specific professional take-home pay.


## Available Tools (4)
- **calculate_price_options**: Calculates the floor price, the recommended price, and the final customer total
- **calculate_provider_net**: Determines exactly how much money the professional earns from a completed transaction
- **generate_pricing_summary**: Provides a complete, high-level overview of all financial aspects for a service in a single call
- **get_cost_breakdown**: Determines the total internal cost of a service before any profit or tax is applied


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salon Service Pricing Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the pricing for a 60-minute hair service with a $30 staff rate, $5 product cost, $10 overhead, 20% target margin, and 8% tax."

**🤖 AI Agent:**
> The price floor is $45.00, the recommended price is $56.25, and the customer total is $60.75.

---

**👤 You:**
> "What is the professional's net pay for a service where the customer pays $100, the recommended price was $90, the commission is 50%, and the internal cost is $40?"

**🤖 AI Agent:**
> The professional's net earnings are $45.00.

---

**👤 You:**
> "Give me a full pricing summary for a 30-minute nail service: $25 staff rate, $8 product cost, $5 overhead, 15% margin, 7% tax, and 40% commission."

**🤖 AI Agent:**
> Price Floor: $20.50, Recommended Price: $24.12, Customer Total: $25.81, Provider Net: $9.65.


## ❓ FAQ

**Q: How does the pricing model handle profit?**
The model uses a target margin percentage to calculate a recommended price that ensures the salon meets its profitability goals after covering all direct and overhead costs.

**Q: Can I calculate just the professional's earnings?**
Yes, you can use the `calculate_provider_net` tool to determine the professional's take-home pay based on the recommended price and their commission percentage.

**Q: What is included in the internal cost?**
The internal cost includes direct labor (based on staff hourly rate and duration), product consumption costs, and the allocated overhead for the service.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/salon-service-pricing-calculator](https://vinkius.com/en/ai-agent-connect/salon-service-pricing-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salon Service Pricing Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `salon-service-pricing-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salon Service Pricing Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salon-service-pricing-calculator": {
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
