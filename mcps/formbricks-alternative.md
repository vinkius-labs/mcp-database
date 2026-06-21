# Formbricks MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/formbricks-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Capture user feedback with open-source surveys that trigger at the right moment inside your product for actionable insights.

## Description
Connect your **Formbricks** environment to any AI agent and simplify your feedback collection and survey management through natural conversation.

### What you can do

- **Survey Control** — List all surveys, check their status, and create or delete survey structures programmatically
- **Response Management** — Query results for any survey to analyze user feedback and submission data
- **People Insights** — List identified contacts and retrieve their metadata and custom attributes
- **Workflow Monitoring** — Inspect configured webhooks and action classes to understand your data flow

### How it works

1. Subscribe to this server
2. Enter your Formbricks Personal API Key
3. Start managing your feedback resources from Claude, Cursor, or any MCP-compatible client


## Available Tools (10)
- **create_survey**: Create a new survey
- **delete_survey**: Delete a survey
- **get_person**: Get details for a specific person
- **get_response**: Get details for a specific response
- **get_survey**: Get details for a specific survey
- **list_action_classes**: List action classes
- **list_people**: List identified people
- **list_responses**: Optionally filter by a specific survey ID.

List survey responses
- **list_surveys**: List all surveys
- **list_webhooks**: List configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Formbricks** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all surveys in Formbricks."

**🤖 AI Agent:**
> I've found 4 surveys: 'Product Feedback', 'NPS Survey', 'Onboarding', and 'Feature Request'.

---

**👤 You:**
> "Show me responses for the NPS survey."

**🤖 AI Agent:**
> Retrieving responses... I found 15 submissions. The average score is 8.5. Notable comments include 'Easy to use' and 'Needs dark mode'.

---

**👤 You:**
> "Get metadata for person 'user_555'."

**🤖 AI Agent:**
> Person 'user_555' is Jane Doe. They are on the 'Pro' plan and have completed 3 surveys in the last month.


## ❓ FAQ

**Q: Can I list all my active surveys using my AI agent?**
Yes! Use the `list_surveys` tool to retrieve a full list of surveys in your Formbricks environment.

**Q: How do I check responses for a specific survey?**
Simply provide the Survey ID to the `list_responses` tool. Your agent will fetch all submissions associated with that survey.

**Q: Can I delete a survey using this agent?**
Yes, use the `delete_survey` action and provide the unique Survey ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/formbricks-alternative](https://vinkius.com/mcp/formbricks-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Formbricks** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `formbricks-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Formbricks** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "formbricks-alternative": {
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
