# Hiveage MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hiveage)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Automate online invoicing via Hiveage — manage invoices, estimates, and payments directly from any AI agent.

## Description
Connect your **Hiveage** account to any AI agent and take full control of your online invoicing, estimates, and customer network through natural conversation.

### What you can do

- **Invoicing Oversight** — List all invoices, retrieve detailed billing data using unique hash keys, and monitor payment status.
- **Estimate Management** — Access your quotations and estimates history to stay on top of pending deals.
- **Payment Recording** — Manually record payments against invoices directly from the chat interface.
- **Customer Network** — List and inspect connections (customers/vendors) in your business network.
- **Document Delivery** — Send invoices to your customers via email with a single command.
- **Tax & Item Visibility** — List saved billing items and tax profiles to ensure accurate invoicing.

### How it works

1. Subscribe to this server
2. Enter your Hiveage API Key and Subdomain
3. Start managing your billing from Claude, Cursor, or any MCP-compatible client

No more manual navigating through complex billing tabs. Your AI assistant acts as a dedicated Billing Manager or Accounts Receivable Specialist.

### Who is this for?

- **Freelancers** — instantly retrieve invoice statuses and record payments while working on projects.
- **Small Business Owners** — automate the process of checking for overdue invoices and sending reminders.
- **Accountants** — quickly list tax profiles and billing items for reconciliation.


## Available Tools (12)
- **record_payment**: Pass details as a JSON string in "body_json" (requires amount, date, and payment_method).

Record a manual payment against an invoice
- **send_invoice_email**: Deliver an invoice to the customer via email
- **get_customer_details**: Get detailed profile information for a network connection
- **get_estimate_details**: Get detailed information about a specific estimate
- **get_invoice_details**: Get detailed information about a specific invoice
- **get_api_profile**: Retrieve information about the authenticated account
- **list_estimates**: List all estimates (quotations) in Hiveage
- **list_invoices**: Use this to monitor billing and find hash keys for specific invoice actions.

List all invoices in your Hiveage account
- **list_billing_items**: List saved items and services used for invoicing
- **list_customers**: List all connections (customers/vendors) in your network
- **list_invoice_payments**: List all payments recorded for a specific invoice
- **list_tax_profiles**: List all configured tax profiles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hiveage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all unpaid invoices and their total amounts."

**🤖 AI Agent:**
> I've retrieved your unpaid invoices. You have 3 pending documents: INV-102 ($450.00), INV-105 ($1,200.00), and INV-110 ($300.00). All are marked as 'SENT' or 'OVERDUE'. Would you like to send a reminder for the overdue invoice?

---

**👤 You:**
> "Record a cash payment of $500 for invoice hash 'kiLDAgtGzNpaAQ'."

**🤖 AI Agent:**
> Payment recorded! I've successfully logged a $500.00 cash payment for invoice kiLDAgtGzNpaAQ. The new balance has been updated in Hiveage. Should I also deliver the updated invoice to the customer?

---

**👤 You:**
> "Show me the details for the estimate with key 'ests_992'."

**🤖 AI Agent:**
> Accessing estimate details... Estimate ests_992 is for 'Website Redesign' totaling $2,500.00. It was sent to 'Acme Corp' last Tuesday and is currently in 'PENDING' status. Would you like to convert this estimate into an invoice?


## ❓ FAQ

**Q: How do I find my Hiveage API Key?**
Log in to your Hiveage account, go to **Settings > API**, and you will find your unique API key there. This key is used as the username for Basic Authentication.

**Q: What is the Hiveage 'Subdomain'?**
The subdomain is the unique part of your Hiveage URL (e.g., if you access Hiveage at `mycompany.hiveage.com`, your subdomain is `mycompany`).

**Q: Can I record a partial payment for an invoice?**
Yes! When using the `record_payment` tool, you can specify any amount in the `body_json`. Hiveage will automatically update the invoice balance based on the recorded payment.

**Q: Is the integration secure for financial data?**
Absolutely. The integration uses official Hiveage API keys over HTTPS. Your credentials and billing data are encrypted and stored securely within the Vinkius Cloud infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hiveage](https://vinkius.com/mcp/hiveage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hiveage** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hiveage` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hiveage** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hiveage": {
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
