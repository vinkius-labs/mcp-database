# Helpshift MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/helpshift)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Automate mobile and web support via Helpshift — manage issues, FAQs, and user profiles directly from any AI agent.

## Description
Connect your **Helpshift** platform to any AI agent and take full control of your customer support and user hub workflows through natural conversation.

### What you can do

- **Issue Oversight** — List all support issues, retrieve detailed metadata, and monitor audit logs for action history.
- **Response Management** — Add messages to existing issues and update statuses (Resolved, Rejected) directly from the chat.
- **Content Insights** — Browse your published FAQ articles and sections to ensure documentation is accurate.
- **User Hub Operations** — Perform bulk user profile updates and creation tasks using the User Hub v2 API.
- **Application Visibility** — List all registered apps in your Helpshift dashboard to ensure correct routing.
- **Operational Efficiency** — Track the progress of bulk identity tasks and monitor support volume in real-time.

### How it works

1. Subscribe to this server
2. Enter your Helpshift API Key and Domain
3. Start managing your support operations from Claude, Cursor, or any MCP-compatible client

No more manual exporting of issue logs. Your AI assistant acts as a dedicated Support Operations Lead or Mobile Support Specialist.

### Who is this for?

- **Support Managers** — instantly retrieve issue transcripts and audit logs to understand complex cases.
- **Mobile Product Teams** — monitor incoming bug reports and user feedback from within the development flow.
- **Customer Success Ops** — automate the management of large user profile batches and identity syncs.


## Available Tools (11)
- **add_issue_message**: Pass the message details as a JSON string in "body_json".

Add a message to an existing issue
- **bulk_user_action**: Pass the actions array as a JSON string in "body_json".

Perform bulk profile operations (v2)
- **create_issue**: Pass the payload as a JSON string in "body_json" (requires app_id, title, body).

Create a new support issue
- **get_issue_audit_logs**: Retrieve the action history for a specific issue
- **get_bulk_task_status**: Check the status of a bulk profile operation
- **get_issue_details**: Get detailed information about a specific issue
- **list_registered_apps**: List all applications registered in your Helpshift dashboard
- **list_faqs**: List all published FAQ articles
- **list_issues**: Useful for monitoring support volume and identifying urgent cases.

List support issues/tickets in Helpshift
- **list_faq_sections**: List FAQ categories/sections
- **update_issue_status**: Update the status of an issue (e.g., Resolved, Rejected)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Helpshift** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active issues and show their audit logs."

**🤖 AI Agent:**
> I've retrieved your active issues. You have 3 open cases, including 'App crash on iOS' (ID: 5501) and 'Payment failure' (ID: 5505). I've also fetched the audit log for 5501, which shows it was reassigned to the Engineering team 2 hours ago. Would you like the full transcript for either case?

---

**👤 You:**
> "Add a reply to issue ID 5501: 'We are investigating the logs now'."

**🤖 AI Agent:**
> Message added! I've successfully sent your reply to issue 5501. The customer will receive this update in their app. Would you like to set the status to 'Resolved' or add any internal tags?

---

**👤 You:**
> "Search for FAQ articles related to 'subscription renewal'."

**🤖 AI Agent:**
> Searching FAQs... I found 2 relevant articles: 'How to renew your plan' and 'Troubleshooting renewal errors'. Would you like the full content of 'How to renew your plan' to share with a customer?


## ❓ FAQ

**Q: How do I find my Helpshift API Key?**
Log in to your Helpshift dashboard, go to **Settings > API**, and you will find your **API Key** listed there. This key is used as the username for Basic Authentication.

**Q: What is the 'Domain' in the setup?**
The domain is the unique identifier for your Helpshift instance (e.g., if you access it at `company.helpshift.com`, your domain is `company`).

**Q: Can I see the history of actions taken on an issue?**
Yes! Use the `get_issue_audit_logs` tool (v2). It retrieves the action history, showing when status was changed, who was assigned, and which tags were added.

**Q: Is the integration secure for support data?**
Absolutely. The integration uses industry-standard Basic Authentication over HTTPS. Your credentials are encrypted and stored securely within the Vinkius Cloud infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/helpshift](https://vinkius.com/mcp/helpshift)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Helpshift** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `helpshift` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Helpshift** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "helpshift": {
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
