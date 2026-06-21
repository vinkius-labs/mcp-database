# SurveyMethods MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/surveymethods)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Online survey software and data analysis.

## Description
The SurveyMethods MCP server empowers your AI agent to manage surveys directly. Query response rates, fetch specific user feedback, and orchestrate automated polls efficiently through your chat.


## Available Tools
- **create_collector**: Create a new collector for a survey
- **create_contact**: Add a new contact
- **create_survey**: Create a new survey
- **delete_survey**: Permanently remove a survey
- **get_me**: Check API connectivity and get account context
- **get_response**: Retrieve a single response by ID
- **get_survey**: Retrieve details for a specific survey
- **list_collectors**: List all collectors (distribution channels) for a survey
- **list_contacts**: List all contacts in your respondent database
- **list_responses**: Retrieve all responses for a specific survey
- **list_surveys**: List all surveys in your account
- **update_survey**: Update an existing survey


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SurveyMethods** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active surveys in my account."

**🤖 AI Agent:**
> You have 2 active surveys: 'Q2 Employee Satisfaction' and 'Product Beta Feedback'.

---

**👤 You:**
> "Get the completion rate for the 'Product Beta Feedback' survey."

**🤖 AI Agent:**
> The survey currently has 150 views and 95 full completions (63.3% completion rate).

---

**👤 You:**
> "Close the survey ID 3042."

**🤖 AI Agent:**
> Survey ID 3042 has been successfully marked as Closed and will no longer accept responses.


## ❓ FAQ

**Q: Can I check the completion rate of a live survey?**
Yes, specify the Survey ID and the agent will extract the current views, starts, and full completions.

**Q: How do I fetch individual user responses?**
You can request the raw data for specific respondents if your integration permissions allow reading payload data.

**Q: Is it possible to close a survey via the AI?**
If write access is enabled, you can command the AI to change a survey's status from 'Open' to 'Closed'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/surveymethods](https://vinkius.com/mcp/surveymethods)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SurveyMethods** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `surveymethods` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SurveyMethods** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surveymethods": {
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
