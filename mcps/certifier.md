# Certifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/certifier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Issue branded digital certificates and badges at scale for courses, events, and achievements that recipients can verify online.

## Description
Connect your **Certifier** account to any AI agent and manage your entire digital credentialing workflow through natural conversation.

### What you can do

- **Credential Lifecycle** — Create, update, issue, and send credentials (certificates, badges, diplomas) to recipients.
- **Template Management** — Browse and inspect credential templates to choose the right structure for each certification.
- **Design Control** — List and review visual design templates that define certificate appearance and branding.
- **Recipient Search** — Search across all credentials by recipient name, email, or custom ID to quickly find records.
- **Status Verification** — Confirm API connectivity and check your total credential count.

### How it works

1. Subscribe to this server
2. Enter your Certifier access token (Settings > Developers > Access Tokens)
3. Start issuing credentials from Claude, Cursor, or any MCP client

### Who is this for?

- **Training Coordinators** — issue completion certificates at scale through simple AI commands.
- **HR Teams** — manage employee certifications and track credentialing status.
- **EdTech Platforms** — automate badge and diploma issuance for course completions.


## Available Tools (12)
- **check_certifier_status**: Verify Certifier API connectivity
- **create_credential**: Requires recipient name, email, and template ID.

Create a new credential for a recipient
- **get_credential**: Get full details of a specific credential
- **get_design_template**: Get details of a specific design template
- **get_credential_template**: Get details of a specific credential template
- **issue_credential**: Once issued, it gets a verification URL and cannot revert.

Issue a draft credential to make it official
- **list_credentials**: List all issued credentials
- **list_design_templates**: List all design templates
- **list_credential_templates**: Use template IDs when creating new credentials.

List all credential templates
- **search_credentials**: Search credentials by recipient name or email
- **send_credential**: Send a credential to the recipient via email
- **update_credential**: Only draft credentials can be modified.

Update an existing credential


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Certifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my credential templates in Certifier."

**🤖 AI Agent:**
> I've found 3 templates: 'Course Completion Certificate' (ID: tpl_8a2bc), 'Workshop Badge' (ID: tpl_9d4ef), and 'Professional Diploma' (ID: tpl_1f6gh). Which template would you like to use for a new credential?

---

**👤 You:**
> "Create a certificate for John Smith (john@example.com) using template tpl_8a2bc."

**🤖 AI Agent:**
> Done! Credential created in draft status (ID: cred_xyz789) for John Smith. Would you like me to issue it now and send it to john@example.com?

---

**👤 You:**
> "Search for all credentials issued to anyone at example.com."

**🤖 AI Agent:**
> I found 5 credentials matching 'example.com': 3 issued, 1 draft, and 1 sent. The most recent is a 'Workshop Badge' issued to Sarah Lee yesterday. Would you like to see the full details for any of these?


## ❓ FAQ

**Q: Can I create a certificate and send it to someone in one workflow?**
Yes! First use `create_credential` with the recipient details and template ID, then `issue_credential` to make it official, and finally `send_credential` to deliver it via email.

**Q: How do I find the right template ID to use when creating a credential?**
Use the `list_credential_templates` tool to browse all available templates. Each template includes its ID, name, and description. Copy the ID and use it in the `create_credential` tool.

**Q: Can I search for a credential by the recipient's email address?**
Absolutely. Use the `search_credentials` tool and enter the recipient's email as the query. It will return all credentials matching that email address.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/certifier](https://vinkius.com/mcp/certifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Certifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `certifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Certifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "certifier": {
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
