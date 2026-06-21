# Basin MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/basin)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/basin-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/basin-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Basin** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/basin](https://vinkius.com/mcp/basin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
