# Conekta MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/conekta)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Equip your AI agent to securely manage Latin American payments, view transactions, and track sales using the Conekta API.

## Description
Integrate your AI assistant with **Conekta**, the leading online payment gateway in Mexico and Latin America. By providing seamless connectivity to your Conekta account, your conversational agent can instantly analyze transaction data, verify specific charges, and keep track of your core e-commerce metrics directly through natural language requests.

### What you can do

- **Transaction Lookups** — Instantly query the status of specific payments by providing a transaction ID or customer email.
- **Sales Analysis** — Ask for summaries of recent successful transactions, refunds, or chargebacks to keep track of store performance.
- **Customer Management** — Retrieve and review customer profiles and their associated payment history to provide faster support.

### How it works

1. Add the Conekta integration to your AI workspace.
2. Secure the connection using your Conekta Private API Key.
3. Chat seamlessly with your agent to pull transaction records, summarize daily sales, and more—without navigating complex dashboards.

### Who is this for?

- **E-commerce Managers** — Rapidly check if a customer's payment has cleared without needing to access the main billing platform.
- **Customer Support Teams** — Instantly verify refund requests and transaction details directly while assisting users.
- **Financial Analysts** — Quickly gather aggregate data on daily revenue, chargebacks, and successful orders.


## Available Tools
- **create_order**: Requires customer name, email, phone, and at least one line item with name, unit_price (in cents), and quantity. Currency defaults to MXN.

Create a new order in Conekta
- **get_customer**: Returns contact info, payment sources, and order history.

Retrieve detailed information about a specific customer
- **get_order**: Returns charges, line items, customer info, and payment status.

Retrieve detailed information about a specific order
- **list_customers**: Retrieve a list of customer records from Conekta
- **list_events**: Useful for debugging integrations.

Retrieve a list of API events (webhook history)
- **list_orders**: Use payment_status filter to narrow results. Supports limit for pagination.

Retrieve a paginated list of orders from Conekta
- **list_subscription_plans**: Retrieve a list of subscription plans in Conekta
- **search_customer_by_email**: Returns matching customer profiles.

Find a Conekta customer by their email address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Conekta** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if the Conekta payment with ID 'ord_2nx...4kx' was successfully processed or declined."

**🤖 AI Agent:**
> The transaction 'ord_2nx...4kx' was successfully processed. It is a charge of $1,250.00 MXN made via credit card. The payment was cleared today at 10:45 AM and the associated customer is 'Carlos Mendoza'.

---

**👤 You:**
> "Summarize today's approved transactions and total revenue in MXN."

**🤖 AI Agent:**
> Today, you have 24 successfully approved transactions through Conekta. The total processed revenue is $34,800.00 MXN. There are also 2 transactions marked as 'declined' due to insufficient funds. Would you like a breakdown of the processing fees?

---

**👤 You:**
> "List the last 5 chargebacks or disputed claims in our account."

**🤖 AI Agent:**
> Here are the 5 most recent chargebacks:
1. ord_9ak - $800.00 MXN (Fraud alert)
2. ord_7bz - $1,200.00 MXN (Unrecognized charge)
3. ord_4cw - $500.00 MXN (Product not received)
4. ord_8dy - $2,500.00 MXN (Duplicate charge)
5. ord_1ex - $350.00 MXN (Fraud alert)
Shall I pull the customer details for ord_9ak?


## ❓ FAQ

**Q: How do I securely obtain my Conekta Private API Key?**
Log in to your Conekta dashboard as an administrator. In the left sidebar, click on 'Developers' (Desarrolladores), then navigate to 'API Keys' (Llaves API). Locate the 'Private Key' (Llave Privada) section—you may need to enter your password to reveal it. Copy this key and paste it into the secure input field below to connect the agent.

**Q: Can the AI agent create new charges or issue refunds directly?**
No. This integration operates strictly in read-only mode to guarantee financial security. The conversational agent can query and extract data regarding transactions, customers, and overall payments, but it cannot authorize new charges or initiate refunds, protecting your account from unintended financial actions.

**Q: What kind of data can I ask the agent to retrieve from Conekta?**
You can ask the agent to check the exact status of a specific payment ID, verify whether a charge was approved or declined, list recent successful orders, or summarize the daily transaction volume and associated processing fees.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/conekta](https://vinkius.com/mcp/conekta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Conekta** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `conekta` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Conekta** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "conekta": {
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
