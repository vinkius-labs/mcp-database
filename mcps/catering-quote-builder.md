# Catering Quote Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/catering-quote-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise catering quotes, labor costs, and profit margins.

## Description
A precision pricing engine for catering professionals. This MCP server connects your AI assistant to specialized tools for calculating event costs. Use `get_menu_pricing` to find ingredient costs, `calculate_service_labor` to determine staffing expenses, and `calculate_logistics_and_rentals` for equipment and delivery. Finally, use `generate_final_quote` to compile all data into a complete customer quote including target margins and taxes.


## Available Tools (4)
- **calculate_logistics_and_rentals**: 
- **calculate_service_labor**: 
- **generate_final_quote**: 
- **get_menu_pricing**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Catering Quote Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the cost for a salmon portion?"

**🤖 AI Agent:**
> The unit cost for the salmon portion is $12.50.

---

**👤 You:**
> "Calculate labor for 4 staff members at $25/hour for 5 hours."

**🤖 AI Agent:**
> The total labor cost is $500.00.

---

**👤 You:**
> "Generate a quote for 50 guests with a $2000 subtotal, 15% margin, and 8% tax."

**🤖 AI Agent:**
> The final customer quote is $2,592.00, with a total profit of $300.00.


## ❓ FAQ

**Q: How do I calculate the total cost for my event?**
You can use `calculate_service_labor` for staff costs and `calculate_logistics_and_rentals` for equipment, then combine them with menu costs using `generate_final_quote`.

**Q: Can I include taxes in the final quote?**
Yes, the `generate_final_quote` tool allows you to specify a `taxRatePercent` to ensure the customer quote is accurate.

**Q: How is profit calculated?**
Profit is calculated by taking the customer quote (excluding taxes) and subtracting all internal costs like food, labor, and logistics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/catering-quote-builder](https://vinkius.com/en/ai-agent-connect/catering-quote-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Catering Quote Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `catering-quote-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Catering Quote Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "catering-quote-builder": {
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
