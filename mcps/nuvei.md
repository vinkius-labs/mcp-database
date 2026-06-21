# Nuvei MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nuvei)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Connect your AI agent to Nuvei to track transactions, manage payments, and securely tokenize cards through natural conversation.

## Description
Connect your **Nuvei** merchant account to your AI agent and manage your global payments platform effortlessly.

### What you can do

- **Payment Processing** — Programmatically invoke the `create_payment` endpoint to handle live orders directly from your chat or workflows.
- **Transaction Auditing** — Query specific payments using `get_payment` or list multiple transactions with `get_transactions` to track settlements and statuses.
- **Card Vaulting & Tokenization** — Securely invoke `create_card_token` without touching raw card data, pushing tokens directly to Nuvei's vault.
- **Token Retrieval** — Look up vaulted payment methods using `get_token` to analyze returning customers or manage subscriptions.

### How it works

1. Subscribe to this server
2. Enter your Nuvei API Credentials and Merchant details
3. Start fetching transaction summaries and creating payments directly from Claude, Cursor, or any AI client

### Who is this for?

- **Finance Teams** — seamlessly fetch daily transaction batches or audit failed payments to reconcile accounting without opening the Nuvei Control Panel.
- **Customer Support** — quickly locate single transactions and verify successful payments for complaining users directly in the CRM workflow.
- **E-commerce Engineers** — tokenize payments and simulate order testing securely without leaving the code editor.


## Available Tools
- **capture_payment**: If amount is omitted, captures the full authorized total.

Capture a previously authorized card payment
- **create_payment**: This initiates a real money authorization/charge network request. Returns the Nuvei transaction ID and status.

Initialize a new payment intent with Nuvei
- **create_card_token**: Tokenize plain card details into a vaulted payment token
- **delete_token**: Stops future recurring charges or 1-click purchases immediately.

Delete a vaulted payment token permanently
- **get_payment**: Essential for checking if an async payment cleared.

Retrieve the current status mapped to a Nuvei Payment ID
- **get_token**: View details of a previously vaulted Nuvei Card/Payment Token
- **get_transactions**: List or enumerate historical transaction records
- **refund_payment**: Supports partial amounts.

Refund a fully captured Nuvei payment
- **update_token**: g. updating an expiry date string) without needing full card details again.

Mutate specific fields inside a vaulted token
- **void_payment**: Note: Can only void pending auths.

Cancel a pending authorized payment preventing capture


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nuvei** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the status of transaction ID 987654321."

**🤖 AI Agent:**
> I've queried Nuvei and the transaction `987654321` was Declined. The Gateway response noted 'Insufficient Funds' on the provided Visa card.

---

**👤 You:**
> "Show me the 10 most recent transactions on my account."

**🤖 AI Agent:**
> Here is a table summarizing your 10 most recent Nuvei transactions. You have 9 Approved charges and 1 Refund in pending status.

---

**👤 You:**
> "Retrieve the token details for Customer UUID `usr-88` in the vault."

**🤖 AI Agent:**
> The vault details for `usr-88` show an active Card Token ending in 4242, expiring 12/28. Would you like me to initiate a new payment using this token?


## ❓ FAQ

**Q: How can I securely pass card inputs if the chat format is plain text?**
The integration routes direct requests to Nuvei's sandbox or live vault using the `create_card_token` feature natively. Since the AI environment is localized and isolated by default, inputs made within Claude or Cursor are ephemeral and pass straight into Nuvei via the secure connection layer without persisting in logs.

**Q: Can I query why a specific transaction was declined?**
Yes. Ask the agent to use `get_payment` with your transaction ID. The AI will parse the complex payload returned by Nuvei and summarize the error message (e.g., Insufficient Funds, Do Not Honor) directly in human language.

**Q: Is it possible to track batch settlements?**
Use the `get_transactions` capability. Your prompt can specify that you want to list out the last 20 payments, and the AI will structure them neatly as a tabular view in your chat interface.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nuvei](https://vinkius.com/mcp/nuvei)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nuvei** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nuvei` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nuvei** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nuvei": {
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
