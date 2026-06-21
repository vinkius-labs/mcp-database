# VATNode MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vatnode)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Validate and audit VAT numbers — identify tax rates and companies via AI.

## Description
Empower your AI agent to orchestrate your entire VAT validation and tax auditing workflow with **VATNode**, the reliable source for global VAT intelligence. By connecting VATNode to your agent, you transform complex tax compliance tasks into a natural conversation. Your agent can instantly verify if a VAT number is valid, audit company registration details, and retrieve current tax rates for any country without you ever touching a manual lookup tool. Whether you are conducting financial due diligence or managing international invoicing, your agent acts as a real-time tax consultant, ensuring your business data is always verified and compliant.

### What you can do

- **VAT Auditing** — Verify if any international VAT number is valid and retrieve detailed company metadata, including names and addresses.
- **Tax Rate Oversight** — Retrieve current standard and reduced VAT rates for any country to maintain a clear view of global tax obligations.
- **Corporate Discovery** — Query company details associated with a VAT number to assist in rapid financial background checks.
- **Global Intelligence** — List VAT rates for all supported countries to understand the reach of different tax systems instantly.
- **Operational Monitoring** — Check your API usage and account metadata to maintain strict control over your research volume.

### How it works

1. Subscribe to this server
2. Enter your VATNode API Key
3. Start managing your tax intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance Managers** — monitor tax compliance and retrieve verified corporate metadata straight from your workflow.
- **Accounting Teams** — verify VAT numbers and audit tax rates for international invoicing without manual searching.
- **Due Diligence Leads** — perform rapid audits of business registration data and identify tax markers through natural language.
- **Operations Leads** — automate tax data querying to orchestrate cross-functional global teams smoothly.


## Available Tools
- **get_company_by_vat**: Retrieve company details associated with a VAT number
- **get_country_tax_info**: Get additional tax information for a country
- **get_api_usage**: Check current VATNode API usage statistics
- **get_country_vat_rates**: Get current VAT rates for a specific country
- **list_all_vat_rates**: List VAT rates for all supported countries
- **validate_vat_number**: Verify if a VAT number is valid and retrieve company metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VATNode** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate the VAT number 'DE123456789' using VATNode."

**🤖 AI Agent:**
> VAT number validated! The ID is valid and corresponds to a registered company in Germany. I've retrieved the company name and address. Would you like the current VAT rates for Germany as well?

---

**👤 You:**
> "What are the standard VAT rates in 'France' (FR)?"

**🤖 AI Agent:**
> I've retrieved the VAT rates for France. The standard rate is 20%. Reduced rates of 10%, 5.5%, and 2.1% are also available for specific categories. I can assist you with more tax auditing if needed.

---

**👤 You:**
> "List all countries with a standard VAT rate above 20%."

**🤖 AI Agent:**
> I've scanned the global rate catalog. Countries with standard rates above 20% include Hungary (27%), Denmark (25%), and Sweden (25%). Would you like the full list of metadata for these countries?


## ❓ FAQ

**Q: How do I find my VATNode API Key?**
Log in to your [**VATNode dashboard**](https://vatnode.dev/dashboard), and you will find your API Key on the main home page. Copy and paste it below.

**Q: Can the agent validate European VAT numbers?**
Yes. VATNode supports validation for VAT numbers across the European Union and several other jurisdictions globally using official VIES data.

**Q: Is tax rate information provided?**
Yes. The `get_country_vat_rates` tool provides current standard and reduced VAT rates, helping you audit tax obligations for different regions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vatnode](https://vinkius.com/mcp/vatnode)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **VATNode** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `vatnode` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **VATNode** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vatnode": {
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
