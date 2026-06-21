# Formstack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/formstack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage professional forms, track submissions, and automate data collection via AI agents with Formstack.

## Description
Connect your **Formstack** account to any AI agent to automate your professional form management and data collection workflows through the Model Context Protocol (MCP). Formstack is the workplace productivity platform used by thousands of organizations to build custom forms, automate manual processes, and securely collect data. This MCP server enables you to manage your form library, retrieve submissions, and oversee fields and webhooks directly through natural conversation.

### Key Features

- **Form Lifecycle** — List all forms in your account, fetch detailed configuration metadata, and create or update forms instantly.
- **Submission Oversight** — Retrieve real-time form submissions, fetch specific data for individual records, and track growth via submission stats.
- **Field Management** — Access and list all fields defined within your forms to understand the data structure and validation rules.
- **Webhook Automation** — Monitor and manage webhooks to receive real-time notifications for every form completion.
- **Embed Support** — Retrieve the raw HTML of any form for quick embedding into external sites or applications.
- **Data Hygiene** — Permanently delete forms or manage active statuses directly through simple AI commands.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Formstack Access Token (found in your API settings)
3. Start managing your professional data collection from Claude, Cursor, or any MCP client

### Who is this for?

- **Compliance Officers** — quickly check submission data or form metadata while ensuring data collection standards are met.
- **Operations Managers** — get a real-time overview of active forms and submission counts through simple AI commands.
- **Marketing Teams** — automate the retrieval of lead data and manage form updates for multi-channel campaigns.


## Available Tools
- **create_form**: Create a new form
- **create_webhook**: Add a webhook
- **delete_form**: Remove a form
- **get_form_html**: Get form raw HTML
- **get_form_stats**: Get form submissions count
- **get_form_details**: Get form metadata
- **get_submission_details**: Get submission data
- **list_form_fields**: List form fields
- **list_forms**: List all forms
- **list_submissions**: List form submissions
- **list_form_webhooks**: List form webhooks
- **update_form**: Update form settings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Formstack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all forms in my Formstack account."

**🤖 AI Agent:**
> Retrieving forms... I found 6 forms, including 'Customer Feedback' and 'Job Application'. Which one would you like to see submissions for?

---

**👤 You:**
> "Show me the 5 most recent submissions for form '1234567'."

**🤖 AI Agent:**
> Fetching submissions... For form 1234567, I found 5 recent submissions. Sentiment appears positive with high scores in 'Service Quality'.

---

**👤 You:**
> "Get the embed HTML code for my 'Survey' form (ID: 9876543)."

**🤖 AI Agent:**
> Retrieving HTML... I've fetched the raw HTML code for form 9876543. You can now copy and paste it into your website's source code.


## ❓ FAQ

**Q: How do I get an Access Token for Formstack?**
You can generate a Personal Access Token in your Formstack account settings under the API section.

**Q: Can I retrieve the raw HTML of a form for embedding?**
Yes! Use the 'get_form_html' tool and provide the Form ID. The agent will return the raw HTML code ready for use.

**Q: Is there a limit to the number of submissions I can retrieve?**
The retrieval depends on your Formstack plan limits. The 'list_submissions' tool supports pagination to help you navigate through large sets of records.

**Q: Can I manage form webhooks through the agent?**
Yes, you can use the 'list_form_webhooks' and 'create_webhook' tools to monitor and automate your real-time data notifications.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/formstack](https://vinkius.com/mcp/formstack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Formstack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `formstack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Formstack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "formstack": {
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
