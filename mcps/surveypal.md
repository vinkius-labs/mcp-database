# Surveypal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/surveypal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Design employee experience surveys and customer feedback programs with analytics that turn responses into actionable improvements.

## Description
Connect your **Surveypal** account to any AI agent and simplify how you collect user data, manage customer feedback loops, and analyze survey results through natural conversation.

### What you can do

- **Survey Management** — List all surveys across your account and folders, and retrieve detailed configuration metadata.
- **Response Analysis** — List and query survey answers with date filtering, and drill down into individual responses.
- **Outreach Automation** — Programmatically send survey invitations via Email or SMS to individual contacts or bulk lists.
- **Organization Control** — Manage survey folders and contact directories to keep your research structured.
- **Operational Monitoring** — Check API health and account status directly from the agent.
- **Data Insights** — Fetch detailed metadata for specific answers to understand customer sentiment via AI.

### How it works

1. Subscribe to this server
2. Enter your Surveypal API Key and API Secret (found in your account integrations)
3. Start managing your feedback ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Experience Managers** — quickly retrieve survey summaries and analyze recent feedback via simple AI queries.
- **Research & Insight Teams** — automate the sending of invitations and verify data availability directly from the workspace.
- **Operations Leads** — monitor survey folders and manage contact directories via the AI assistant.


## Available Tools
- **get_account_info**: Get account info
- **get_answer**: Get individual answer
- **get_contact**: Get contact details
- **get_api_status**: Check API status
- **get_survey**: Get survey details
- **list_survey_answers**: List survey answers
- **list_contacts**: List survey contacts
- **list_folder_surveys**: List surveys in folder
- **list_folders**: List survey folders
- **list_surveys**: List all surveys
- **send_email_invitation**: Send email invitation
- **send_sms_invitation**: Send SMS invitation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surveypal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active surveys in my Surveypal account."

**🤖 AI Agent:**
> I've retrieved your surveys. You have 3 active surveys: 'Customer Satisfaction Q4', 'Product Beta Feedback', and 'Event Registration'. Which one would you like to see responses for?

---

**👤 You:**
> "Show me the last 5 answers for the 'Customer Satisfaction' survey."

**🤖 AI Agent:**
> I've fetched the latest answers. Most users provided positive feedback, highlighting the new checkout flow. However, two respondents mentioned slow load times. Shall I retrieve the full text for those specific answers?

---

**👤 You:**
> "Send an email invitation for survey '10293' to 'user@example.com'."

**🤖 AI Agent:**
> Invitation sent! I've triggered the email for survey 10293 to user@example.com. The recipient will receive the link to participate shortly.


## ❓ FAQ

**Q: Can I see all the answers for a specific survey via AI?**
Yes! Use the `list_survey_answers` tool and provide the Survey ID. Your agent will retrieve a list of all submissions, which you can then ask the AI to summarize or filter.

**Q: How do I send a survey invitation via SMS using the agent?**
Use the `send_sms_invitation` action. Provide the Survey ID and a JSON array of phone numbers. The agent will trigger the SMS broadcast instantly via Surveypal.

**Q: Is it possible to list surveys from a specific folder via AI?**
Absolutely. Use the `list_folder_surveys` query and provide the Folder ID. The agent will retrieve all surveys organized within that specific directory.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/surveypal](https://vinkius.com/mcp/surveypal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surveypal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `surveypal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surveypal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surveypal": {
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
