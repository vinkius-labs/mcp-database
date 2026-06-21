# Formsite MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/formsite)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage forms, retrieve results, and automate data collection via AI agents with Formsite.

## Description
Connect your **Formsite** account to any AI agent to automate your form results retrieval and data management through the Model Context Protocol (MCP). Formsite is a professional form builder that enables organizations to create sophisticated forms and surveys. This MCP server allows you to list your forms, fetch real-time results, and manage webhooks directly through natural conversation.

### What you can do

- **Results Retrieval** — List and fetch form submissions/results instantly, including detailed answers and timestamps.
- **Form Oversight** — Access and list all forms in your account to maintain full visibility of your active data collectors.
- **Field Inspection** — Retrieve the fields and items defined within your forms to understand the structure of your data.
- **Webhook Automation** — Create and manage webhooks to receive real-time notifications when new results are completed.
- **Reporting Insights** — List and retrieve reports defined for your forms to get high-level snapshots of your data.
- **Multi-Server Support** — Seamlessly connect to your specific Formsite server environment (e.g., fs18).

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Formsite Server, User Directory, and Access Token (found in Settings > Integrations > Formsite API)
3. Start managing your form data from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Analysts** — quickly pull form results for analysis or list report metadata without leaving your primary agent.
- **Operations Teams** — automate the monitoring of new form submissions and webhook configurations.
- **Customer Feedback Managers** — manage sophisticated surveys and retrieve user sentiment via simple AI commands.


## Available Tools
- **create_webhook**: Create a new webhook
- **delete_webhook**: Remove a webhook
- **get_form_details**: Get form metadata
- **get_form_reports**: Get form reports
- **list_form_items**: List form fields
- **list_forms**: List all forms
- **list_results**: List form results
- **list_webhooks**: List form webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Formsite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all forms in my Formsite account and their directory names."

**🤖 AI Agent:**
> Retrieving forms... I found 5 forms, including 'Annual Survey' (dir: survey_2023) and 'Contact Form' (dir: contact_us). Which one would you like to check results for?

---

**👤 You:**
> "Show me the 10 most recent results for form 'survey_2023'."

**🤖 AI Agent:**
> Fetching results... For survey_2023, I found 10 recent submissions. Key feedback includes requests for 'Faster shipping' and 'More color options'.

---

**👤 You:**
> "What fields are defined in my 'Contact' form (dir: contact_us)?"

**🤖 AI Agent:**
> Inspecting form items... The 'Contact Form' includes fields for 'Name', 'Email Address', 'Subject', and 'Message (Paragraph Text)'.


## ❓ FAQ

**Q: How do I get an Access Token for Formsite?**
You can find your Access Token in your Formsite account by going to Form Settings > Integrations > Formsite API.

**Q: What is the 'Server' and 'User Directory' required for setup?**
The Server is your prefix (e.g., fs18) and the User Directory is your account name. Both are displayed on the Formsite API integration page.

**Q: Can I receive real-time notifications for new form results?**
Yes! Use the 'create_webhook' tool to subscribe a URL to the 'result_completed' event for any of your forms.

**Q: Are the results returned in JSON format?**
Yes, all data retrieved through this MCP server is provided in a structured format, which the AI agent can then summarize for you.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/formsite](https://vinkius.com/mcp/formsite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Formsite** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `formsite` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Formsite** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "formsite": {
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
