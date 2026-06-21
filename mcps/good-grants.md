# Good Grants MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/good-grants)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Discover and manage grant applications with a platform that matches your organization to the right funding opportunities.

## Description
Connect your **Good Grants** account to any AI agent and simplify how you coordinate your grant programs, track applicant data, and monitor the review process through natural conversation.

### What you can do

- **Application Oversight** — List all grant applications and retrieve detailed metadata, status, and custom field values.
- **Review & Scoring** — List and query application reviews and scores to monitor the evaluation progress.
- **Fund Management** — List available grant funds and programs to coordinate your funding distribution.
- **User & Applicant CRM** — Manage your directory of users and team members registered in the system.
- **Categorization** — List and query grant categories to organize your programs and maintain a structured database.
- **Operational Automation** — Create new grant applications programmatically and verify configurations via AI commands.
- **Real-time Status** — Check the progress of individual applications and verify reviewer assignments directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Good Grants API Key (found in your account settings)
3. Start managing your grant lifecycle from Claude, Cursor, or any MCP client

### Who is this for?

- **Program Managers & Grant Officers** — quickly check application statuses and monitor scoring progress via simple AI queries.
- **Operations Teams** — manage fund distributions and verify applicant metadata directly from the workspace.
- **Reviewers & Evaluators** — verify assigned applications and retrieve review history via the AI assistant.


## Available Tools
- **create_new_application**: Register a new application
- **get_application_details**: Get details for a specific application
- **list_applications**: List Good Grants applications
- **list_grant_categories**: List grant categories
- **list_grant_funds**: List grant funds
- **list_application_reviews**: List reviews
- **list_account_users**: List account users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Good Grants** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active grant applications in my account."

**🤖 AI Agent:**
> I've retrieved your applications. You have 25 active submissions including 'Community Garden Project', 'Tech for Good Grant', and 'Startup Seed Fund'. Which one would you like to see the details or status for?

---

**👤 You:**
> "Show me the reviews and scores for application 'app_10293'."

**🤖 AI Agent:**
> Fetching reviews... For application app_10293, I found 3 reviews with an average score of 8.5/10. Reviewers highlighted the 'Social Impact' as a strong point. Shall I retrieve the full comments?

---

**👤 You:**
> "Create a new application titled 'Youth Tech Workshop' in the 'Education' category."

**🤖 AI Agent:**
> Success! The application 'Youth Tech Workshop' has been created in your Good Grants account (ID: app_88231). It is currently in draft status in the 'Education' category.


## ❓ FAQ

**Q: Can I see the scores for a specific application via AI?**
Yes! Use the `list_application_reviews` tool. Your agent will retrieve the history of scores and comments provided by the reviewers for that application.

**Q: How do I create a new grant application using the agent?**
Use the `create_new_application` action. Provide the Fund ID, Category ID, and the application title. The agent will instantly register the draft in your Good Grants account.

**Q: Is it possible to list all registered applicants via AI?**
Absolutely. Use the `list_account_users` query. The agent will retrieve the complete directory of users and applicants stored in your platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/good-grants](https://vinkius.com/mcp/good-grants)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Good Grants** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `good-grants` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Good Grants** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "good-grants": {
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
