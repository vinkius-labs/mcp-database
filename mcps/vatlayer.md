# Vatlayer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vatlayer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Validate EU VAT numbers and retrieve real-time VAT rates for EU member states to ensure global tax compliance.

## Description
Connect **Vatlayer** to your AI agent to automate VAT number validation and tax rate calculations across the European Union through natural conversation.

### What you can do

- **VAT Validation** — Instantly verify any EU VAT number using the `validate_vat` tool and retrieve official company details and addresses.
- **Rate Retrieval** — Fetch current VAT rates for specific countries using `get_rate` or get the full list for all EU member states with `get_rate_list`.
- **Price Calculation** — Use `calculate_price` to perform country-specific and VAT-compliant price calculations based on amount and product type.
- **IP-Based Localization** — Automatically determine applicable VAT rates based on custom IP addresses or client location.

### How it works

1. Subscribe to this server
2. Enter your Vatlayer Access Key
3. Start validating taxes and calculating rates from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Developers** — Automate tax calculations during checkout flows and verify customer tax IDs directly from the IDE.
- **Accountants & Finance Teams** — Quickly verify the validity of vendor VAT numbers and audit tax rates without manual lookups.
- **SaaS Platforms** — Ensure global billing compliance by integrating real-time tax data into automated workflows.


## Available Tools (4)
- **calculate_price**: Perform country-specific and VAT compliant price calculations
- **get_rate_list**: Request a full set of VAT rates for all EU member states
- **get_rate**: Request VAT rates for a specific EU member state
- **validate_vat**: Validate an EU VAT number


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vatlayer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate the VAT number LU26375245 and tell me which company it belongs to."

**🤖 AI Agent:**
> I've validated the VAT number LU26375245. It is a valid number belonging to 'Amazon Europe Core S.à r.l.' located in Luxembourg.

---

**👤 You:**
> "What is the current standard VAT rate in Germany?"

**🤖 AI Agent:**
> Fetching VAT rates for Germany (DE)... The current standard VAT rate is 19%. There are also reduced rates of 7% for certain goods.

---

**👤 You:**
> "Calculate the total price including VAT for 150 EUR in France."

**🤖 AI Agent:**
> Based on a base amount of 150 EUR and the French standard VAT rate of 20%, the VAT amount is 30 EUR, making the total price 180 EUR.


## ❓ FAQ

**Q: How can I check if a specific EU VAT number is valid and active?**
Use the `validate_vat` tool by providing the VAT number (e.g., LU26375245). The agent will return the validation status along with company name and address details.

**Q: Can I get a complete list of VAT rates for all EU member states at once?**
Yes, simply run the `get_rate_list` tool. It will fetch the full set of VAT rates for all 28 EU member states in a single response.

**Q: How do I calculate a VAT-compliant price for a specific country?**
Use the `calculate_price` tool. Provide the base amount and the 2-letter country code. You can also specify a product type (like 'medical') to apply reduced rates if applicable.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vatlayer](https://vinkius.com/mcp/vatlayer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vatlayer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vatlayer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vatlayer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vatlayer": {
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
