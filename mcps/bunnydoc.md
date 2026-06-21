# BunnyDoc MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bunnydoc)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Manage eSignatures via BunnyDoc — track document status, manage templates, and coordinate signature requests directly from any AI agent.

## Description
Connect your **BunnyDoc** account to any AI agent and orchestrate your eSignature workflows, document lifecycle, and team collaboration through natural conversation.

### What you can do

- **Signature Requests** — Trigger new document signature requests using pre-defined templates directly from your workspace.
- **Status Oversight** — Monitor the real-time status of envelopes (Draft, Sent, Signed, Completed) using natural language.
- **Template Management** — List all available document templates to ensure consistency in your signing workflows.
- **Team Coordination** — Access your directory of team members and invite new collaborators to the platform.
- **Webhook Automation** — Subscribe to lifecycle events (viewed, signed, completed) to automate your back-office response.
- **Document Auditing** — Retrieve detailed metadata and audit trails for any envelope ID straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your BunnyDoc API Key
3. Start managing your eSignatures from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations & Legal Teams** — quickly check if a contract is signed or send new requests without manual portal work.
- **HR Managers** — monitor onboarding document completion and team access straight from their workflow tools.
- **Developers** — integrate legal signing steps into their environment using natural language.


## Available Tools
- **add_team_member**: Invite a new member to the team
- **create_signature_request**: Create a new signature request from a template
- **get_account_info**: Retrieve core account information
- **get_envelope_status**: Get status of a specific signature request (envelope)
- **get_usage_stats**: Retrieve API usage statistics
- **list_envelopes**: List all signature requests
- **list_team_members**: List all members of the team
- **list_templates**: List all available document templates
- **subscribe_webhook**: Subscribe to signature events via webhook
- **unsubscribe_webhook**: Remove a webhook subscription


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BunnyDoc** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my document templates in BunnyDoc."

**🤖 AI Agent:**
> I've retrieved your templates. You have 3 templates: 'Employment Agreement' (ID: temp_1), 'NDA' (ID: temp_2), and 'Sales Contract' (ID: temp_3).

---

**👤 You:**
> "Show the status of signature request env_99283."

**🤖 AI Agent:**
> The status for request env_99283 ('NDA - John Doe') is 'Completed'. All parties have signed the document as of March 20th.

---

**👤 You:**
> "Send the 'NDA' template to Jane Smith (jane@example.com)."

**🤖 AI Agent:**
> Signature request for the 'NDA' template has been sent to Jane Smith. The new envelope ID is env_12345.


## ❓ FAQ

**Q: Can I check if a document has been signed using the agent?**
Yes! Use the `get_envelope_status` tool with the Envelope ID. Your agent will fetch the current status (e.g., 'Completed' or 'Sent') directly from BunnyDoc.

**Q: How do I send a signature request to multiple recipients?**
Simply ask the agent to `create_signature_request` and provide the Template ID and a JSON array of recipients. Each object should include the recipient's name and email.

**Q: Does the integration allow listing all available templates?**
Yes. Use the `list_templates` tool. It will retrieve all the document templates configured in your BunnyDoc account, making it easy to find the ID you need for a new request.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bunnydoc](https://vinkius.com/mcp/bunnydoc)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BunnyDoc** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bunnydoc` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BunnyDoc** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bunnydoc": {
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
