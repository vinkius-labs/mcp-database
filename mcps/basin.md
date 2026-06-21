# Basin MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/basin)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Form backend and lead capture automation — manage form submissions, filter spam, and trigger webhooks via AI.

## Description
Empower your AI agent to orchestrate your entire lead capture workflow with **Basin**, the powerful form backend for modern websites. By connecting Basin to your agent, you transform static submission data into a natural conversation. Your agent can instantly audit new form entries, identify and flag spam, retrieve specific lead details, and even manually refire webhooks without you ever touching a dashboard. Whether you're managing a single contact page or a complex lead generation network, your agent acts as a real-time submission manager, ensuring your inbound data is always clean and actionable.

### What you can do

- **Submission Management** — List all form submissions across your account or dive deep into specific entry details via natural language.
- **Spam Control** — Instantly mark suspicious entries as spam or unmark false positives to maintain a high-quality lead database.
- **Form Oversight** — List all forms in your Basin account and retrieve detailed metadata for each to map your data collection points.
- **Webhook Triggers** — Manually refire webhooks for specific submissions to ensure your downstream integrations are correctly updated.
- **Real-time Auditing** — Retrieve the single latest submission instantly to respond to new leads with zero delay.

### How it works

1. Subscribe to this server
2. Enter your Basin API Key
3. Start managing your form submissions through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — audit new campaign leads and filter through submissions through natural conversation.
- **Customer Support Teams** — quickly retrieve details from contact form entries to prepare responses for new inquiries.
- **Operations Leads** — monitor form activity and verify webhook delivery status directly from your chat interface.
- **Developers** — integrate reliable form backend management into AI-driven data processing workflows.


## Available Tools (12)
- **delete_submission**: Permanently delete a submission
- **get_account_check**: Verify Basin connection
- **get_form**: Get details for a specific form
- **get_latest_submission**: Retrieve the single most recent submission
- **get_submission**: Get full details for a specific submission
- **list_form_submissions**: Helper to list submissions for a specific form
- **list_forms**: List all forms in your Basin account
- **list_submissions**: List all submissions across all forms
- **mark_as_not_spam**: Convenience tool to unmark a submission as spam
- **mark_as_spam**: Convenience tool to mark a submission as spam
- **refire_webhooks**: Manually trigger webhooks for a specific submission
- **update_submission**: Update submission metadata (e.g. mark as spam)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Basin** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the latest submission from my contact forms."

**🤖 AI Agent:**
> I've retrieved the latest submission. It's from 'John Doe' (john@example.com) via the 'Contact Us' form. He is interested in a product demo. Would you like the full details?

---

**👤 You:**
> "Mark submission ID 'sub_abc123' as spam."

**🤖 AI Agent:**
> Submission `sub_abc123` has been successfully marked as spam. It will no longer appear in your active lead list.

---

**👤 You:**
> "List all forms in my Basin account."

**🤖 AI Agent:**
> I've found 3 forms in your account: 'Contact Page', 'Newsletter Signup', and 'Ebook Download'. Which one would you like to audit?


## ❓ FAQ

**Q: How can I check the latest lead that submitted a form?**
Use the `get_latest_submission` tool. It automatically retrieves the single most recent entry across all your forms, allowing you to respond instantly.

**Q: Can the agent filter out spam submissions?**
Yes. Use the `mark_as_spam` tool with a Submission ID to flag suspicious entries. You can also use `mark_as_not_spam` to restore entries that were incorrectly flagged.

**Q: Is it possible to re-send data to my CRM if it failed?**
Yes. Use the `refire_webhooks` tool by providing the Submission ID. This manually triggers any webhooks associated with that form, ensuring your external integrations receive the data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/basin](https://vinkius.com/mcp/basin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Basin** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `basin` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Basin** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "basin": {
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
