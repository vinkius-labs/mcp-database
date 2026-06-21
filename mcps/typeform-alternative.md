# Typeform MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/typeform-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Create beautifully designed forms and surveys that ask one question at a time and get dramatically higher completion rates.

## Description
Connect your **Typeform** account to any AI agent and simplify how you collect data, manage surveys, and analyze user responses through natural conversation.

### What you can do

- **Form Management** — List all forms across your account and retrieve detailed field structures and logic.
- **Response Analysis** — List and export individual submissions with filtering by date and completion status.
- **Workspace Oversight** — Manage workspaces to keep your forms and surveys organized by project or team.
- **Real-time Monitoring** — Create and manage webhooks to receive instant notifications for new form submissions.
- **Design Control** — List available themes to ensure consistent branding across your surveys.
- **Integration Maintenance** — Verify account configurations and regional settings directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Typeform Personal Access Token and select your Region (US or EU)
3. Start managing your forms and data from Claude, Cursor, or any MCP client

### Who is this for?

- **Researchers & Analysts** — quickly retrieve survey responses and analyze trends via simple AI commands.
- **Marketing Teams** — monitor lead generation forms and verify submission counts directly from the workspace.
- **Product Managers** — get instant bird's-eye views of user feedback and workspace organization via the AI assistant.


## Available Tools
- **create_webhook**: Requires a unique tag and a destination URL.

Create or update a form webhook
- **get_form_details**: Essential for understanding the questions asked in a form.

Get details and structure for a specific form
- **get_workspace_details**: Get details and forms for a workspace
- **list_forms**: Useful for obtaining form IDs for response retrieval.

List all Typeforms in the account
- **list_responses**: Supports filtering by date (since) and completion status.

List all collected responses for a form
- **list_design_themes**: List all available design themes
- **list_webhooks**: Webhooks are used to receive real-time alerts when a form is submitted.

List all webhooks for a specific form
- **list_workspaces**: Workspaces are used to organize collections of forms.

List all Typeform workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Typeform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active forms in my Typeform account."

**🤖 AI Agent:**
> I've retrieved your forms. You have 5 active surveys including 'Customer Satisfaction 2024', 'Lead Intake Form', and 'Employee Engagement'. Which one would you like to see responses for?

---

**👤 You:**
> "Show me the last 5 responses for the 'Customer Satisfaction' form."

**🤖 AI Agent:**
> I've fetched the latest submissions. There are 5 recent responses. Most users seem happy with the new UI, but 2 mentioned issues with the payment step. Shall I retrieve the detailed comments?

---

**👤 You:**
> "List all forms in the 'Marketing Campaign' workspace (ID: 10293)."

**🤖 AI Agent:**
> Fetching forms... The 'Marketing Campaign' workspace contains 3 forms: 'Newsletter Sign-up', 'Product Interest Quiz', and 'Webinar Registration'. Shall I check the submission count for any of these?


## ❓ FAQ

**Q: Can I see the individual responses for a specific form?**
Yes! Use the `list_responses` tool and provide the 8-character Form ID. You can also filter by date using the `since` parameter to see only recent submissions.

**Q: How do I find the questions and fields defined in a form?**
Use the `get_form_details` query. Your agent will retrieve the complete structure of the form, including all question texts, field types, and logic transitions.

**Q: Is it possible to configure a webhook via AI to track new leads?**
Absolutely. Use the `create_webhook` action. Provide the Form ID, a custom tag, and your destination URL to start receiving real-time notifications for each submission.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/typeform-alternative](https://vinkius.com/mcp/typeform-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Typeform** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `typeform-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Typeform** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "typeform-alternative": {
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
