# EU VAT Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eu-vat-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate EU VAT rates, transaction taxes, and compliance rules for 27 member states.

## Description
An essential engine for managing European Union Value Added Tax (VAT) complexity. This MCP server provides specialized tools to navigate the regulatory landscape of the 27 EU member states. Use `lookup_vat_rate` to find specific tax percentages based on country and product category, including standard, reduced, and super-reduced tiers. The `compute_transaction_tax` tool automates calculations for domestic sales, B2C cross-border (OSS), and B2B reverse charge scenarios, providing the exact tax amount and total invoice value. Additionally, use `check_vat_compliance` to verify if a transaction follows the correct regulatory path like 'Domestic VAT', 'Reverse Charge', or 'OSS'. This tool is ideal for developers building e-commerce platforms or accounting software operating within the EU.


## Available Tools (3)
- **check_vat_compliance**: Identify the VAT rule applied to a transaction
- **lookup_vat_rate**: g., DE, FR) and a product category (Standard Goods, Reduced Goods, or Essential Goods).

Look up the VAT rate for a country and product category
- **compute_transaction_tax**: Calculate VAT amount and total for a transaction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EU VAT Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the VAT rate for food in France?"

**🤖 AI Agent:**
> The applicable VAT rate for 'Reduced Goods' in France (FR) is 5.5%.

---

**👤 You:**
> "Calculate the total for a €100 sale from Italy to Spain for a consumer."

**🤖 AI Agent:**
> For a B2C transaction from IT to ES with a net amount of €100.00, the applied rate is 21%. The tax amount is €21.00, making the total amount €121.00 under the OSS rule.

---

**👤 You:**
> "Is a B2B sale from Germany to Ireland subject to reverse charge?"

**🤖 AI Agent:**
> Yes, the transaction follows the 'Reverse Charge' rule because it is a cross-border B2B sale.


## ❓ FAQ

**Q: How do I find the VAT rate for a specific product in Germany?**
Use the `lookup_vat_rate` tool by providing 'DE' as the country code and specifying the appropriate category, such as 'Standard Goods', 'Reduced Goods', or 'Essential Goods'.

**Q: Does this tool handle B2B transactions between different EU countries?**
Yes. By using `compute_transaction_tax` with the 'B2B' transaction type and differing origin/destination country codes, the tool will identify the Reverse Charge mechanism and return a zero tax amount.

**Q: How can I verify if a transaction follows OSS rules?**
You can use the `check_vat_compliance` tool. By setting `isCrossBorder` to true and `isBusinessBuyer` to false, the tool will confirm if the 'OSS' rule applies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eu-vat-calculator](https://vinkius.com/mcp/eu-vat-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EU VAT Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `eu-vat-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EU VAT Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eu-vat-calculator": {
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
