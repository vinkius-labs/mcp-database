# Attraction Ticket Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/attraction-ticket-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate total revenue, tax impact, and tiered pricing for attraction visitors.

## Description
This MCP server provides tools to manage attraction revenue by calculating final totals, evaluating tax impacts, and summarizing tiered pricing. Use `get_total_revenue` to find the final amount including tax and discounts, `validate_visitor_eligibility` to check group requirements, `calculate_tax_impact` to see tax costs, and `get_tiered_pricing_summary` for category breakdowns.


## Available Tools (4)
- **get_total_revenue**: Calculates the final total amount to be paid by a group of visitors
- **calculate_tax_impact**: Evaluates how much the total cost increases due to different tax rates
- **get_tiered_pricing_summary**: Provides a breakdown of costs when different types of visitors are present
- **validate_visitor_eligibility**: Determines if a specific visitor count can be processed under specific pricing rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Attraction Ticket Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost for 10 visitors if the ticket price is 50, the tax rate is 0.05, and there is a 5 discount?"

**🤖 AI Agent:**
> The total amount is 472.50. This includes a subtotal of 450.00 and a tax amount of 22.50.

---

**👤 You:**
> "How many more people do I need to reach a group size of 15 if I have 10 visitors?"

**🤖 AI Agent:**
> You need 5 more visitors to reach the minimum group size of 15.

---

**👤 You:**
> "Show me the pricing breakdown for 2 adults at 100 each and 3 children at 50 each."

**🤖 AI Agent:**
> The total subtotal is 350.00. The breakdown is: adult: 200.00, child: 150.00.


## ❓ FAQ

**Q: How do I calculate the final price for a group?**
You can use the `get_total_revenue` tool by providing the visitor count, base ticket price, tax rate, and any applicable discount.

**Q: Can I check if a group qualifies for a discount?**
Yes, use the `validate_visitor_eligibility` tool to determine if the visitor count meets the minimum group size requirement.

**Q: How is tax calculated?**
The `calculate_tax_impact` tool calculates the tax amount and the total including tax based on the subtotal and the decimal tax rate provided.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/attraction-ticket-calculator](https://vinkius.com/en/ai-agent-connect/attraction-ticket-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Attraction Ticket Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `attraction-ticket-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Attraction Ticket Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "attraction-ticket-calculator": {
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
