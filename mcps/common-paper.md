# Common Paper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/common-paper)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Common Paper helps you create, send, and sign standard commercial contracts faster. Use this MCP server to automate your contract workflow and track agreement status.

## Description
Connect your **Common Paper** account to any AI agent and manage your commercial contracts through natural conversation.

### What you can do

- **Agreement Management** — List all signed agreements, check the status of pending contracts, and retrieve details for any specific document.
- **Contract Creation** — Send new agreements such as NDAs, Cloud Service Agreements (CSA), and DPAs directly to partners using predefined templates.
- **Workflow Automation** — Streamline your internal processes by programmatically fetching agreement data and triggering contract actions.

### How it works

1. Subscribe to this server
2. Enter your Common Paper API Key
3. Start managing your contracts through Claude, Cursor, or any MCP-compatible client

No more manual drafting or navigating complex legal platforms. Your AI agent becomes your contracting assistant.

### Who is this for?

- **Sales Teams** — quickly send out NDAs or Service Agreements to prospects and track signatures without leaving your workflow.
- **Legal Operations** — audit executed contracts and monitor agreement statuses across the organization.
- **Founders & Executives** — streamline the legal boilerplate required to close deals faster.


## Available Tools (10)
- **create_webhook**: Configure a new webhook to receive contract status updates
- **delete_webhook**: Remove a previously configured webhook
- **get_agreement**: Retrieve detailed information about a specific agreement
- **get_template**: Retrieve details of a specific contract template
- **list_agreements**: Retrieve a list of agreements (contracts) from Common Paper
- **list_signed_agreements**: Quickly list all agreements that have been fully signed
- **list_templates**: Retrieve a list of contract templates available in your account
- **list_webhooks**: Retrieve a list of configured webhooks
- **search_agreements_by_email**: Find agreements associated with a specific recipient email
- **send_agreement**: Create and send a new agreement based on a template


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Common Paper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all signed agreements in Common Paper."

**🤖 AI Agent:**
> I found 5 signed agreements in your Common Paper account. Would you like me to display their details?

---

**👤 You:**
> "Send an NDA agreement to 'partner@example.com' using template ID 'tmpl-xxxx' in Common Paper."

**🤖 AI Agent:**
> I've successfully sent the NDA agreement to 'partner@example.com'. The agreement status is currently pending signature.

---

**👤 You:**
> "Get the current status of agreement 'agr-yyyy' in Common Paper."

**🤖 AI Agent:**
> The agreement 'agr-yyyy' is currently fully executed. It was signed on March 15, 2026.


## ❓ FAQ

**Q: How do I get my Common Paper API key?**
You can generate an API key in your Common Paper account under Settings > Integrations.

**Q: Which agreement types are supported?**
Common Paper supports standard contracts like NDAs, Cloud Service Agreements (CSA), and Data Processing Agreements (DPA).

**Q: Can I use custom templates?**
Yes, you can use any template created in your Common Paper account by providing its unique template ID to the 'send_agreement' tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/common-paper](https://vinkius.com/mcp/common-paper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Common Paper** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `common-paper` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Common Paper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "common-paper": {
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
