# SurveySparrow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/surveysparrow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Collect feedback with conversational surveys that feel like chat and boost completion rates across employee and customer programs.

## Description
Connect your **SurveySparrow** account to any AI agent and simplify how you collect multi-channel feedback, manage your audience directory, and analyze survey data through natural conversation.

### What you can do

- **Survey Oversight** — List all conversational surveys, retrieve detailed configuration metadata, and query question structures.
- **Response Analysis** — List and query survey submissions with status filtering (completed/started) to monitor completion rates.
- **Audience Management** — Manage your CRM contacts, create new profiles, and organize them into contact lists for targeted sharing.
- **Campaign Tracking** — List email shares and invitations to monitor how your surveys are being distributed.
- **Webhook Integration** — List active webhooks to ensure your event-driven workflows are active and notifying correctly.
- **Operational Visibility** — Check account status, verify region settings, and manage contact lifecycles directly via AI.

### How it works

1. Subscribe to this server
2. Enter your SurveySparrow Access Token and select your Region (US, EU, EU-DEV, etc.)
3. Start managing your experience management ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Experience Managers** — quickly retrieve survey summaries and analyze customer sentiment via simple AI commands.
- **Marketing & Outreach Teams** — manage contact lists and monitor survey share statuses directly from the workspace.
- **Operations Analysts** — verify response data and completion metrics via the AI assistant.


## Available Tools (12)
- **create_contact**: Add new contact
- **remove_contact**: Delete contact
- **get_user_profile**: Get account info
- **get_contact_info**: Get contact details
- **get_survey_questions**: List survey fields
- **get_survey_details**: Get survey info
- **list_contact_folders**: List contact lists
- **list_crm_contacts**: List audience contacts
- **list_survey_responses**: List survey submissions
- **list_email_shares**: List survey invitations
- **list_surveys**: List SurveySparrow surveys
- **list_active_webhooks**: Get notifications config


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SurveySparrow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active surveys in my SurveySparrow account."

**🤖 AI Agent:**
> I've retrieved your surveys. You have 3 active conversational surveys: 'Customer Effort Score', 'Product Pulse Check', and 'New Feature Survey'. Which one would you like to see responses for?

---

**👤 You:**
> "Show me the last 5 responses for the 'Customer Effort Score' survey."

**🤖 AI Agent:**
> I've fetched the latest responses. There are 5 recent submissions. Completion rate is 80%, with most users taking about 2 minutes to finish. Shall I retrieve the detailed answers?

---

**👤 You:**
> "Search for a contact with the email 'jane.doe@example.com'."

**🤖 AI Agent:**
> I've found the record. Jane Doe (ID: cont_10293) is a registered contact in your CRM. She is currently in the 'Loyal Customers' list. Would you like to see her full survey history?


## ❓ FAQ

**Q: Can I see all the questions in a survey via AI?**
Yes! Use the `get_survey_questions` tool and provide the Survey ID. Your agent will retrieve the complete structure, including labels and field types.

**Q: How do I list all the contacts stored in my account?**
Run the `list_crm_contacts` query. The agent will retrieve a list of all audience members stored in your SurveySparrow account.

**Q: Is it possible to see the status of survey responses (started vs completed)?**
Absolutely. Use the `list_survey_responses` tool and provide the Survey ID. You can pass the optional `state` parameter to filter by completion status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/surveysparrow](https://vinkius.com/mcp/surveysparrow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SurveySparrow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surveysparrow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SurveySparrow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surveysparrow": {
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
