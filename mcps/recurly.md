# Recurly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/recurly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Equip your AI to directly manage subscriptions, billing accounts, and invoices within your Recurly ecosystem without shifting interfaces.

## Description
Connect your **Recurly** subscription billing and management platform securely to your conversational AI agent. Activating this integration transforms your AI into a dynamic revenue operations assistant, giving it the autonomy to look up accounts, adjust active subscription states, and analyze invoice pipelines directly from the terminal.

### What you can do

- **Account Management** — Quickly list your customer directory, view detailed billing profiles, or instantly create a new account mapping without opening the vendor console.
- **Subscription Operations** — Easily search and read subscription lifecycle states, enroll users in fresh catalog plans, un-cancel previous subscriptions, or permanently cancel an ongoing billing mandate.
- **Invoice & Plan Catalogs** — Retrieve the list of historical generated invoices to verify successful automated payments or pull all active billing models (Catalog Plans) to review available products.

### How it works

1. Add the Recurly MCP server to your authorized module list.
2. Configure the server using your specific Recurly subdomain alongside your Private API Key.
3. Chat seamlessly with your AI to process operations like revoking a subscription instance or querying for a customer's missing invoice.

### Who is this for?

- **RevOps & Finance Teams** — Pull billing analytics, track active subscription statuses, and instantly generate plan insights via conversational commands during reviews.
- **Customer Support Agents** — Quickly verify if an account holds a successful invoice payment or pause/cancel client subscriptions mid-chat without escalating to billing engineers.
- **Software Developers** — Interact safely with Recurly limits, list the ID structures of catalog plans, and test provisioning logic endpoints directly from the code editor.


## Available Tools
- **cancel_subscription**: This action is irreversible.

Cancels an active subscription
- **create_account**: Specify code, email, and name.

Creates a new customer account
- **create_subscription**: Creates a new subscription for an account
- **get_account_details**: Retrieves details for a specific customer account
- **get_subscription_details**: Retrieves details for a specific subscription
- **list_accounts**: Lists all customer accounts in Recurly
- **list_catalog_plans**: Lists all available subscription plans in the product catalog
- **list_invoices**: Lists all generated invoices
- **list_subscriptions**: Lists all subscriptions managed by Recurly
- **reactivate_subscription**: Reactivates a previously cancelled or expired subscription


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recurly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 invoices generated in our account."

**🤖 AI Agent:**
> I executed `list_invoices` restricted to 5 items. The returned set includes invoice IN_UUID_1012 ($59.00 - Paid) and IN_UUID_1013 ($199.00 - Pending).

---

**👤 You:**
> "Cancel the subscription with ID 'sub_39xjd82kw0'."

**🤖 AI Agent:**
> Running the `cancel_subscription` tool. The subscription 'sub_39xjd82kw0' has been set to cancel. It will not renew at the end of the current billing cycle.

---

**👤 You:**
> "Retrieve the billing details for account code 'cus_alpha_92'."

**🤖 AI Agent:**
> I invoked `get_account_details` for 'cus_alpha_92'. The account corresponds to 'Alpha Corp'. It currently has an active subscription to the 'Enterprise Tier' and zero past due payments.


## ❓ FAQ

**Q: How do I find my Subdomain and API Key?**
Your subdomain is the first part of your Recurly portal URL (e.g., if you log in at `myproject.recurly.com`, your subdomain is `myproject`). To get your API Key, navigate inside Recurly to Integrations > API Credentials and generate or copy your 'Private API Key'.

**Q: Can it accidentally charge my customers?**
While the server can manage subscriptions (e.g., setting up a customer with a plan), it strictly follows the billing logic predefined in your Recurly catalog settings. It doesn't bypass credit card validation or execute arbitrary charges directly without a plan context.

**Q: Does cancelling a subscription remove the account entirely?**
No, using `cancel_subscription` stops future renewals for that specific plan item instance. The underlying user billing account remains intact and can hold other valid subscriptions or past invoices.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/recurly](https://vinkius.com/mcp/recurly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Recurly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `recurly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Recurly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recurly": {
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
