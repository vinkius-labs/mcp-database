# Paperform MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/paperform)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-operations](../categories/business-operations.md)

Manage online forms and submissions via Paperform — list forms, track submissions, and configure webhooks directly from any AI agent.

## Description
Connect your **Paperform** account to any AI agent and take full control of your data collection workflows through natural conversation.

### What you can do

- **Form Oversight** — List all forms, retrieve detailed configurations, and manage your form library.
- **Submission Tracking** — List and retrieve detailed data for form submissions to analyze responses in real-time.
- **Webhook Management** — List and create webhooks for your forms to integrate with other services effortlessly.
- **Organizational Visibility** — List folders and custom domains to maintain a clear view of your account structure.
- **Metadata Auditing** — List all tags used across your forms to ensure consistent categorization.

### How it works

1. Subscribe to this server
2. Enter your Paperform Access Token (from Account Settings > API)
3. Start managing your forms directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing Operations** — quickly check form submission counts or verify webhook configurations.
- **Customer Research** — retrieve and analyze form responses without leaving your chat interface.
- **Developers** — audit form metadata and integration settings during implementation.


## Available Tools
- **create_webhook**: Create a new webhook for a form
- **get_account_info**: Get authenticated account information
- **get_form**: Get details for a specific form
- **get_submission**: Get details for a specific submission
- **list_custom_domains**: List all custom domains configured
- **list_folders**: List all form folders
- **list_forms**: List all Paperform forms
- **list_submissions**: List submissions for a form
- **list_tags**: List all tags used in the account
- **list_webhooks**: List webhooks for a form


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paperform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all forms in my Paperform account."

**🤖 AI Agent:**
> I've retrieved 8 forms, including 'Contact Us', 'Product Feedback', and 'Event Registration'. Which one would you like to see submissions for?

---

**👤 You:**
> "Show me the last 5 submissions for the 'Event Registration' form."

**🤖 AI Agent:**
> I've fetched the latest 5 submissions. They include responses from 'John Doe', 'Jane Smith', and 3 others. Would you like the full details for any of these?

---

**👤 You:**
> "List all webhooks configured for form 'form_12345'."

**🤖 AI Agent:**
> There are 2 webhooks for this form: one pointing to Zapier and another to a custom endpoint (https://api.example.com/webhook).


## ❓ FAQ

**Q: How do I find my Paperform Access Token?**
In your Paperform account, go to **Account Settings** > **API**. There you can create and manage your API access tokens.

**Q: Can I see individual form responses?**
Yes! Use the `list_submissions` tool to see a list of responses for a specific form, and `get_submission` to retrieve the full data for a particular entry.

**Q: Does this support webhook management?**
Absolutely. You can use the `list_webhooks` and `create_webhook` tools to monitor and configure integrations for any of your forms.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/paperform](https://vinkius.com/mcp/paperform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paperform** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `paperform` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paperform** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paperform": {
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
