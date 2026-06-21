# Yousign MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yousign)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Manage electronic signatures, signers, and document requests on Yousign — the leading eSignature platform for European teams.

## Description
Connect your **Yousign** account to any AI agent and manage your electronic signature infrastructure through natural conversation.

### What you can do

- **Signature Lifecycle** — Create new signature requests in draft mode, add signers, and activate requests to send them for signing
- **Request Monitoring** — List and browse all signature processes and retrieve real-time status (draft, ongoing, done, cancelled)
- **Signer Management** — Define and add multiple signers to a request by providing their contact details directly from your agent
- **Document Discovery** — List all files attached to a specific signature request to verify the contents before activation
- **Cancellation Control** — Permanently stop ongoing signature requests and provide custom reasons for termination through simple commands
- **Quota Auditing** — Retrieve API consumption and credit details to monitor your Yousign plan usage and remaining signatures
- **Deep Discovery** — Quickly find unique request, signer, and document IDs required for automated legal workflows

### How it works

1. Subscribe to this server
2. Enter your Yousign API Key
3. Start managing your signing processes through Claude, Cursor, or any MCP-compatible client

No more manual logging into the Yousign dashboard to check if a document was signed. Your AI agent becomes your legal operations assistant.

### Who is this for?

- **Legal & Compliance Teams** — monitor signature statuses and audit document requests through simple chat commands
- **HR Managers** — automate signing processes for employment contracts and verify signer completion via chat
- **Sales Professionals** — track contract signatures and activate new signing requests without manual navigation
- **Operations Managers** — monitor API consumption and manage document lifecycles efficiently


## Available Tools
- **list_requests**: Lists all signature requests in the Yousign organization
- **get_request**: Retrieves details and status for a specific signature request
- **create_request**: Provide a descriptive name for the request.

Creates a new signature request in draft mode
- **add_signer**: Provide the request ID and signer contact details.

Adds a new signer to an existing draft signature request
- **activate_request**: This triggers email notifications to all signers.

Activates a draft signature request and sends it to signers
- **cancel_request**: Provide the request ID and an optional reason for cancellation.

Permanently cancels an ongoing signature request
- **list_documents**: Lists all documents attached to a specific signature request
- **get_consumption**: Retrieves API consumption and quota details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Yousign** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all ongoing signature requests in Yousign."

**🤖 AI Agent:**
> I found 3 ongoing requests: 1. 'Partnership Agreement' (ID: req-101), 2. 'Employment Contract - John' (ID: req-102), and 3. 'Vendor Terms' (ID: req-103). Would you like to see the signer status for any of these?

---

**👤 You:**
> "Add 'Jane Smith' (jane@example.com) as a signer to request ID 'req-101'."

**🤖 AI Agent:**
> Success! I've added Jane Smith as a signer to the 'Partnership Agreement' (req-101). Would you like to add more signers or activate the request now?

---

**👤 You:**
> "Check our current API consumption and credits."

**🤖 AI Agent:**
> You have consumed 45 out of 100 signatures in your current billing cycle. You have 55 signature credits remaining. Would you like me to list the most recent signed documents?


## ❓ FAQ

**Q: Can I check the status of a signature request via chat?**
Yes. The `get_signature_request` tool allows your AI agent to retrieve the real-time status of any request ID, showing you whether it is in 'draft', 'ongoing', 'done', or has been 'cancelled'.

**Q: How do I add signers to a draft request using the agent?**
You can use the `add_signer` tool. Provide the unique request ID along with the signer's email, first name, and last name. You can add multiple signers to a single request before activating it.

**Q: Can I see how many signature credits I have left in my plan?**
Absolutely. Use the `get_api_consumption` tool to retrieve your current usage statistics and remaining signature credits, helping you manage your Yousign subscription budget.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yousign](https://vinkius.com/mcp/yousign)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Yousign** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `yousign` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Yousign** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "yousign": {
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
