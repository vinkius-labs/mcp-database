# Zoho Invoice MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-invoice)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage billing invoices, estimates, and customer contacts via the Zoho Invoice API.

## Description
Connect your **Zoho Invoice** account to any AI agent to streamline your business billing and client management. This MCP server enables your agent to interact with professional invoices, quotes (estimates), and customer data directly from natural language interfaces.

### What you can do

- **Invoicing Control** — List, retrieve, and create professional invoices for your products and services
- **Estimate Oversight** — Access all quotes and price approximations sent to your customers to track sales leads
- **Item Management** — Query your product and service catalog, including pricing and metadata
- **Customer CRM** — Manage detailed customer profiles and retrieve their contact information instantly
- **Multi-Business Support** — List all organizations associated with your account and manage invoicing data by organization ID

### How it works

1. Subscribe to this server
2. Enter your Zoho Client ID, Client Secret, and Data Center Domain
3. Start managing your billing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Freelancers & Small Businesses** — Quickly generate invoices and check payment statuses via natural language
- **Billing Specialists** — Automate the retrieval of estimates and maintain customer records effortlessly
- **Developers** — Integrate professional invoicing data and billing automation into your custom workflows


## Available Tools (7)
- **list_invoice_contacts**: List all contacts (customers)
- **create_new_invoice**: Requires a JSON body with invoice details.

Create a new invoice
- **list_estimates**: List all estimates (quotes) for an organization
- **get_invoice_details**: Get details for a specific invoice
- **list_invoices**: List all invoices for an organization
- **list_invoice_items**: List all items (products/services)
- **list_organizations**: Use this to identify the organization ID for other calls.

List all Zoho Invoice organizations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho Invoice** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all organizations in my Zoho Invoice account."

**🤖 AI Agent:**
> I've retrieved your organizations. You have 2 entities: 'Freelance Services (ID: 123456)' and 'Design Agency (ID: 789012)'. Which one would you like to access?

---

**👤 You:**
> "Show my 5 most recent invoices for organization ID '123456'."

**🤖 AI Agent:**
> For organization 123456, I found 5 recent invoices. The latest is INV-1001 for $500.00, currently marked as 'Sent'. The previous one was INV-1000 for $1,250.00, marked as 'Paid'.

---

**👤 You:**
> "List all customers in organization '123456'."

**🤖 AI Agent:**
> I've retrieved your customer list. You have 12 active customers, including 'Tech Solutions', 'Global Ventures', and 'Alice Smith'. Would you like more details for any of them?


## ❓ FAQ

**Q: How do I find my Organization ID?**
Use the `list_organizations` tool to retrieve all businesses registered in your account along with their unique IDs.

**Q: Which Data Center domains are supported?**
You can use Zoho domains such as `com` (US), `eu` (Europe), `in` (India), `com.au` (Australia), or `jp` (Japan).

**Q: Can I create an estimate directly via the agent?**
While the current action tool is for invoices, you can retrieve existing estimates using `list_estimates`. Support for creating estimates can be added upon request.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-invoice](https://vinkius.com/mcp/zoho-invoice)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zoho Invoice** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zoho-invoice` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zoho Invoice** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zoho-invoice": {
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
