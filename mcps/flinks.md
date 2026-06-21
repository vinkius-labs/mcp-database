# Flinks MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flinks)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Connect to financial institutions to aggregate banking data, verify income, and perform deep transaction analysis via Flinks.

## Description
Connect your **Flinks** instance to any AI agent to access real-time banking data, verify financial health, and automate KYC workflows through natural conversation.

### What you can do

- **Account Aggregation** — Retrieve full account details, balances, and transaction history from thousands of supported financial institutions.
- **Income Verification** — Use `get_income_attributes` to analyze income stability, sources, and verification patterns automatically.
- **Credit & Risk Analysis** — Fetch consumer or business analysis attributes to understand credit risk and financial behavior.
- **Transaction Categorization** — Automatically categorize bank transactions to understand spending patterns and merchant data.
- **Document Retrieval** — Fetch original bank-issued PDF statements (Canada only) for auditing and compliance.

### How it works

1. Subscribe to this server
2. Enter your Flinks Instance, Customer ID, API Key, and Secret Key
3. Start querying financial data directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Fintech Developers** — Test and integrate banking data flows without leaving the code editor.
- **Lending & Credit Teams** — Instantly analyze income and risk attributes for loan applications.
- **Accounting Professionals** — Automate the retrieval of transaction summaries and categorized data for reconciliation.


## Available Tools
- **authorize_session**: Authenticate a session and fetch cached banking data
- **create_transaction**: Requires FLINKS_CLIENT_ID credential.

Create an EFT transaction (debit or credit)
- **delete_card**: Delete all data associated with a specific user account
- **field_match**: Verify customer identity by comparing details against bank data
- **generate_authorize_token**: Valid for 30 minutes.

Generate a one-time authorize token
- **get_accounts_detail_async**: Poll for asynchronous account details processing
- **get_accounts_detail**: If 202 is returned, data is processing and you should poll the async endpoint.

Retrieve full account details including transactions and KYC
- **get_accounts_summary**: Retrieve general account details and balances
- **get_business_analysis_attributes**: Get insights for business underwriting and creditworthiness
- **get_categorization**: Get categorized transaction data
- **get_income_attributes**: Get income verification and stability insights
- **get_statements**: Retrieve original bank-issued PDF statements (Canada Only)
- **get_user_analysis_attributes**: Get credit-risk use-case attributes for a consumer
- **list_institutions**: List all available financial institutions supported by Flinks
- **set_scheduled_refresh**: Enable or disable nightly refreshes for a specific account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flinks** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all supported financial institutions in Canada."

**🤖 AI Agent:**
> I've retrieved the list of institutions for Canada. Major ones include RBC Royal Bank, TD Canada Trust, and Scotiabank. Would you like the full list or details for a specific one?

---

**👤 You:**
> "Analyze the income stability for the account linked to RequestId 'req_12345'."

**🤖 AI Agent:**
> Using the `get_income_attributes` tool, I've analyzed the data. The user has a stable monthly income of approximately $4,500 from 'TechCorp Inc', with consistent deposits over the last 6 months.

---

**👤 You:**
> "Get the categorized transactions for RequestId 'req_67890'."

**🤖 AI Agent:**
> I've fetched the categorization data. Significant spending categories include 'Housing' (35%), 'Groceries' (15%), and 'Transportation' (10%). Would you like a detailed breakdown of the 'Groceries' category?


## ❓ FAQ

**Q: What should I do if get_accounts_detail returns a 202 status?**
A 202 status means the operation is pending. You should use the `get_accounts_detail_async` tool with the same RequestId to poll for the data until it is ready.

**Q: Can I filter the list of supported financial institutions by country?**
Yes. Use the `list_institutions` tool and provide a comma-separated list of country codes (e.g., 'CA,US') in the `countries` parameter.

**Q: How do I start a new data retrieval session?**
First, run `generate_authorize_token` to get a 30-minute token. Then, use `authorize_session` with that token and the user's LoginId to establish the connection.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flinks](https://vinkius.com/mcp/flinks)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flinks** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `flinks` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flinks** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flinks": {
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
