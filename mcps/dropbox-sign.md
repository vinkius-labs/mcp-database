# Dropbox Sign MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dropbox-sign)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage e-signature requests, track document status, and monitor templates via the Dropbox Sign (HelloSign) API.

## Description
Integrate **Dropbox Sign** (formerly HelloSign), the intuitive e-signature platform, directly into your AI workflow. Manage your outbound signature requests, track signer status and document completion, monitor your reusable signature templates, and oversee your document workflows using natural language.

### What you can do

- **Request Oversight** — List and retrieve detailed information and completion status for all your e-signature requests.
- **Signer Intelligence** — Monitor real-time signer statuses, email addresses, and event logs for every document in your pipeline.
- **Template Management** — Access and monitor all reusable signature templates configured in your account, including role definitions and merge fields.
- **Workflow Auditing** — Retrieve high-level summaries of signature volumes, completion rates, and outstanding documents requiring attention.

### How it works

1. Connect the Dropbox Sign integration to your AI assistant.
2. Authorize using your Dropbox Sign (HelloSign) API Key (found in your account settings).
3. Orchestrate your document signing and e-signature workflows through intuitive conversation.

### Who is this for?

- **Operations Managers** — Quickly check signature statuses and outstanding document volumes on the go.
- **HR & Legal Teams** — Monitor employee onboarding documents and contract completions via chat.
- **Sales Operations** — Research specific request details and signer history to accelerate deals instantly.


## Available Tools
- **get_dropbox_sign_account_metadata**: Retrieve metadata and usage limits for your Dropbox Sign account
- **quick_signature_volume_audit**: Retrieve a high-level summary of signature request activity and completion rates
- **get_signature_request_details**: Get detailed information and signature status for a specific request
- **get_template_configuration**: Get detailed settings and field definitions for a specific template
- **list_outstanding_signatures**: Identify signature requests that are currently awaiting signatures
- **list_latest_signature_requests**: Identify the most recently created signature requests
- **list_signature_requests**: List all signature requests in your Dropbox Sign account
- **list_signature_templates**: List all reusable signature templates configured in your account
- **list_templates_by_signer_role**: Identify templates that include specific signer roles (mock logic)
- **search_signature_requests**: Search for signature requests using a keyword or query string


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dropbox Sign** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all outstanding signature requests."

**🤖 AI Agent:**
> I've found 4 outstanding requests, including 'Sales Contract - Tech Corp' and 'Employee Onboarding - Jane Doe'. Would you like to see the signer status for the Tech Corp contract?

---

**👤 You:**
> "Show me the details for signature request 'REQ-12345'."

**🤖 AI Agent:**
> Request 'REQ-12345' (Title: Partnership Agreement) is 'Awaiting Signatures'. Signer 1 (John Smith) has signed, but Signer 2 (Alice Jones) has only viewed the document. Should I send a reminder to Alice?

---

**👤 You:**
> "List all reusable signature templates."

**🤖 AI Agent:**
> You have 5 active templates, including 'Standard NDA', 'Service Level Agreement', and 'Consulting Contract'. Would you like to see the signer roles defined for the NDA template?


## ❓ FAQ

**Q: How do I get a Dropbox Sign API Key?**
Log in to your Dropbox Sign (HelloSign) account, navigate to **Settings > API**, and you can generate or retrieve your unique API Key from there. Note that API access may require a specific plan.

**Q: Can the agent send new signature requests?**
This integration currently focuses on listing and auditing signature requests and templates. Sending new requests with document uploads should be managed via the Dropbox Sign web portal or mobile app.

**Q: Does the integration show specific signer statuses?**
Yes, you can use the get_signature_request_details tool to see exactly who has signed, who is pending, and any specific events like views or declines.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dropbox-sign](https://vinkius.com/mcp/dropbox-sign)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dropbox Sign** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dropbox-sign` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dropbox Sign** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dropbox-sign": {
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
