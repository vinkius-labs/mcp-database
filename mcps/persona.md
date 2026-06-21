# Persona MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/persona)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage identity verification workflows via Persona — handle inquiries, manage accounts, and inspect verifications directly from your AI agent.

## Description
Connect your **Persona** dashboard to any AI agent to streamline your identity verification and KYC/AML compliance workflows through natural conversation.

### What you can do

- **Inquiry Management** — List, retrieve, and process identity verification inquiries. Approve or decline submissions based on automated or manual reviews.
- **Account Orchestration** — Create, update, and list account entities to maintain a clear record of verified users and their associated data.
- **Verification Inspection** — Fetch detailed verification results and metadata to understand the status of specific identity checks.
- **Privacy & Compliance** — Use redaction tools to permanently delete PII from accounts and inquiries, ensuring compliance with data protection regulations like GDPR.
- **Data Analysis** — Query inquiry lists with pagination and filtering to generate reports on verification throughput.

### How it works

1. Subscribe to this server
2. Enter your Persona API Secret Key
3. Start managing identity flows from Claude, Cursor, or any MCP-compatible client

No more jumping between dashboards to check if a user has submitted their ID. Your AI acts as a compliance assistant, ready to audit and action verifications instantly.

### Who is this for?

- **Compliance Officers** — quickly review inquiry statuses and redact sensitive data without manual spreadsheet tracking
- **Support Teams** — verify user account status and inquiry progress directly during customer interactions
- **Developers** — test and inspect verification flows and account updates straight from the terminal or IDE


## Available Tools (27)
- **approve_inquiry**: Approve an Inquiry
- **create_account**: Create an Account
- **create_inquiry**: Create an Inquiry
- **create_transaction**: Create a Transaction
- **create_webhook**: Create a Webhook
- **decline_inquiry**: Decline an Inquiry
- **get_account**: Retrieve an Account
- **get_case**: Retrieve a Case
- **get_event**: Retrieve an Event
- **get_inquiry**: Retrieve an Inquiry
- **get_report**: Retrieve a Report
- **get_transaction**: Retrieve a Transaction
- **get_verification**: Retrieve a Verification
- **list_accounts**: List all Accounts
- **list_cases**: List all Cases
- **list_events**: List all Events
- **list_inquiries**: List all Inquiries
- **list_reports**: g., Watchlists, Adverse Media).

List all Reports
- **list_transactions**: List all Transactions
- **list_webhooks**: List all Webhooks
- **redact_account**: Redact an Account
- **redact_inquiry**: Redact an Inquiry
- **redact_report**: Redact a Report
- **redact_verification**: Redact a Verification
- **set_case_status**: Set Status on a Case
- **trigger_workflow**: Create a Workflow Run
- **update_account**: Update an Account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Persona** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent 10 identity inquiries."

**🤖 AI Agent:**
> I've retrieved the latest inquiries. There are 10 records found, including Inquiry inq_123abc (Status: completed) and inq_456def (Status: pending). Would you like to inspect the details of the pending one?

---

**👤 You:**
> "Get the account details for account ID acc_789ghi."

**🤖 AI Agent:**
> Fetching account acc_789ghi... This account is associated with user 'Jane Doe', created on 2023-10-12, and currently has 2 completed verifications linked to it.

---

**👤 You:**
> "Approve inquiry inq_456def."

**🤖 AI Agent:**
> Processing approval for inq_456def... The inquiry has been successfully approved. The user's status has been updated in the Persona dashboard.


## ❓ FAQ

**Q: Can I manually approve or decline a verification inquiry through the AI?**
Yes. You can use the `approve_inquiry` or `decline_inquiry` tools by providing the specific Inquiry ID. This allows you to take immediate action on pending verifications based on your review.

**Q: How do I handle GDPR or privacy requests to delete user data?**
The server includes `redact_account` and `redact_inquiry` tools. These actions permanently delete Personally Identifiable Information (PII) associated with the specified ID, helping you maintain compliance with privacy regulations.

**Q: Can I see the specific details of why a verification failed?**
By using the `get_verification` tool with a Verification ID, you can retrieve the full metadata and results of a check, which typically includes status codes and reasonings for the verification outcome.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/persona](https://vinkius.com/mcp/persona)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Persona** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `persona` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Persona** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "persona": {
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
