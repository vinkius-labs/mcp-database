# Pylon MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pylon)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate B2B support and CRM via Pylon — manage issues, accounts, and knowledge bases with AI.

## Description
Connect your **Pylon CRM** (getpylon.com) account to any AI agent and take full control of your customer support and post-sales orchestration through natural conversation. Pylon provides a specialized platform for managing B2B relationships directly within shared channels like Slack and Microsoft Teams, and this integration allows you to retrieve issue metadata, manage account profiles, and search knowledge bases directly from your chat interface.

### What you can do

- **Issue & Ticket Orchestration** — List all managed support issues and retrieve detailed metadata, including creating new issues programmatically.
- **Account & Contact Control** — Access and monitor your customer accounts and retrieve profile metadata via natural language to maintain a clear overview of your client base.
- **Conversation Intelligence** — Retrieve and analyze message threads within specific issues to understand customer intent and provide synthesized summaries.
- **Knowledge Base Integration** — Access and search through your organization's knowledge bases to find relevant documentation directly from the AI interface.
- **Operational Monitoring** — Track organization-wide support health and manage custom field metadata using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your Pylon API Token from your dashboard settings
3. Start managing your customer support from Claude, Cursor, or any MCP-compatible client

No more manual issue tracking or switching between support channels. Your AI acts as a dedicated support specialist or customer success lead.

### Who is this for?

- **Customer Success Managers** — quickly retrieve issue summaries and monitor account health without switching apps.
- **B2B Support Teams** — automate the retrieval of message history and reply to issues via natural conversation.
- **Operations Teams** — streamline the retrieval of account metadata and monitor organizational support performance directly within the chat.


## Available Tools
- **create_issue**: Pass data as a JSON string.

Create a new issue
- **get_account**: Get details for a specific customer account
- **get_issue_messages**: Retrieve messages for an issue
- **get_issue**: Get details for a specific support issue
- **list_accounts**: List all customer accounts
- **list_articles**: List knowledge base articles
- **list_issues**: List all Pylon issues
- **list_knowledge_bases**: List all knowledge bases
- **list_tags**: List all available issue tags
- **reply_to_issue**: Send a reply to an issue
- **update_issue**: Update a support issue


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pylon** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all open issues in my Pylon account."

**🤖 AI Agent:**
> I've retrieved your issues. You have 3 open support tickets including 'Integration bug' and 'Billing question'. Would you like to see the messages for any of them?

---

**👤 You:**
> "Show me all open support issues assigned to the engineering team sorted by priority."

**🤖 AI Agent:**
> 18 open issues assigned to Engineering. Critical (3): "API rate limiting not working" (Acme Corp, 4 hours old), "Data sync failure" (TechFlow, 6 hours), "Authentication timeout" (Meridian, 2 days). High (7): includes payment processing delays, webhook delivery issues, and SDK compatibility bugs. Medium (5): feature requests and configuration questions. Low (3): documentation corrections. Average first response time: 23 minutes. SLA compliance: 94%.

---

**👤 You:**
> "Reply to the Acme Corp API rate limiting issue with a status update and estimated resolution time."

**🤖 AI Agent:**
> Reply sent to Acme Corp issue #ISS-4521. Message: "Hi team, we've identified the root cause of the rate limiting issue. A configuration change in our load balancer was incorrectly throttling requests below the documented limits. A fix has been deployed to staging and is being validated. ETA for production: within 2 hours." Status updated to: In Progress. Priority maintained: Critical. Internal note added for the engineering team with the specific config change details.


## ❓ FAQ

**Q: Can my AI automatically find the latest messages for a specific support issue?**
Yes! Use the `get_issue_messages` tool with the Issue ID. Your agent will respond with the complete metadata for the conversation thread, including sender details and timestamps in seconds.

**Q: How do I find my Pylon API Token?**
Log in to your Pylon dashboard, navigate to **Settings** > **API** (or `app.getpylon.com/settings/api`), and you will find or generate your unique secret token there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pylon](https://vinkius.com/mcp/pylon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pylon** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pylon` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pylon** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pylon": {
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
