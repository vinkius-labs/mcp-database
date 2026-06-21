# PagBank PagSeguro MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pagbank-pagseguro)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Create Pix, Boleto, and Card payment links, and manage transactions via PagBank API.

## Description
Connect **PagBank (PagSeguro)** to any AI agent and unlock Brazil's leading payment solutions — generate Pix QR codes, Boleto payments, and checkout links for credit cards through natural conversation.

### What you can do
- **Instant Pix** — Generate Pix payments with QR Code data for instant confirmation
- **Boleto Generation** — Create Boleto Bancário for customers without credit cards
- **Checkout Links** — Generate payment links that support Credit Card installments
- **Transaction Search** — Find payments by date range or reference code
- **Refunds** — Cancel transactions (full or partial) easily
- **Account Balance** — Check your current available balance
- **Installments** — Calculate credit card installment options

### How it works
1. Subscribe to this server
2. Enter your PagBank Production or Sandbox Access Token
3. Start processing payments and managing your finances from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Brazilian Sellers** — Accept payments via Pix and Boleto instantly from your AI assistant
- **E-commerce Managers** — Monitor transactions, check balances, and issue refunds via chat
- **Developers** — Integrate PagBank payments into AI workflows without complex SDKs


## Available Tools
- **get_balance**: Get the current account balance
- **create_boleto_payment**: Generate a Boleto payment
- **cancel_transaction**: If amount is provided, performs partial cancellation.

Cancel a transaction (full or partial refund)
- **create_checkout_link**: Returns a code and a URL.

Create a payment link (checkout) for multiple items
- **get_order**: Get details of an order by ID
- **get_transaction**: Get details of a transaction by code
- **get_installment_options**: Get installment options for a card brand
- **create_pix_payment**: Create an instant Pix payment
- **search_transactions**: Search for transactions by date range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PagBank PagSeguro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a Pix payment of R$99.90 for reference 'ORDER-001'."

**🤖 AI Agent:**
> Pix payment created! Status: WAITING. QR Code generated for user to scan.

---

**👤 You:**
> "Show me the balance of my account."

**🤖 AI Agent:**
> Current Available Balance: R$ 1,250.45.

---

**👤 You:**
> "Cancel transaction 12345-ABCDE-67890."

**🤖 AI Agent:**
> Transaction cancelled successfully! Status: CANCELLED.


## ❓ FAQ

**Q: How do I get a PagBank Access Token?**
Log in to your [**PagBank Account**](https://pagseguro.uol.com.br). Go to **Account > Credentials** (or Developer section) and generate your **Production Token**. Copy the token and paste it below.

**Q: Can I generate Pix payments?**
Yes! Use the `create_pix_payment` action. It returns the QR Code data (Base64 and copy-paste text) that you can display for the user to pay instantly.

**Q: Does it support Boleto?**
Yes! Use the `create_boleto_payment` action. You need to provide the payer's Name and CPF to generate the Boleto link and barcode.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pagbank-pagseguro](https://vinkius.com/mcp/pagbank-pagseguro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PagBank PagSeguro** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pagbank-pagseguro` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PagBank PagSeguro** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pagbank-pagseguro": {
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
