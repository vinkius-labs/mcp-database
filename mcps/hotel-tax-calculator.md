# Hotel Tax Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hotel-tax-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise hotel taxes, VAT, and occupancy fees for USA and Europe.

## Description
This MCP server provides specialized tools for calculating hotel accommodation taxes and fees across various jurisdictions in the USA and Europe. It allows AI agents to accurately determine tax rates using `get_tax_rate`, compute specific tax amounts with `calculate_room_tax`, generate detailed tax lists via `get_tax_breakdown`, and verify regional compliance with `validate_jurisdiction_rules`. It is designed to handle complex scenarios involving VAT in Europe and various occupancy taxes in the USA.


## Available Tools (4)
- **get_tax_breakdown**: The taxList must be a JSON string representing an array of objects with name and rate.

Provide a detailed list of all taxes and surcharges applied to a stay
- **get_tax_rate**: Find the applicable tax percentage for a specific location
- **validate_jurisdiction_rules**: Check if a specific tax application is legal or standard within a given region
- **calculate_room_tax**: Compute the exact tax amount owed for a stay


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hotel Tax Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the tax rate for VAT in France?"

**🤖 AI Agent:**
> The standard VAT rate in France is 20%.

---

**👤 You:**
> "Calculate the tax for a $250 room with a 12% tax rate."

**🤖 AI Agent:**
> The tax amount is $30.00, making the total $280.00.

---

**👤 You:**
> "Is 'CityTax' a valid tax type in New York City?"

**🤖 AI Agent:**
> Yes, CityTax is a recognized tax type in New York City.


## ❓ FAQ

**Q: How do I find the tax rate for a specific city?**
You can use the `get_tax_rate` tool by providing the city name and the type of tax you are looking for.

**Q: Can I get a full breakdown of multiple taxes?**
Yes, the `get_tax_breakdown` tool allows you to pass a list of taxes to see the individual amount for each and the final grand total.

**Q: Does this support European VAT?**
Yes, the server is designed to handle both European VAT and USA-based occupancy taxes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hotel-tax-calculator](https://vinkius.com/en/ai-agent-connect/hotel-tax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hotel Tax Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hotel-tax-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hotel Tax Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hotel-tax-calculator": {
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
