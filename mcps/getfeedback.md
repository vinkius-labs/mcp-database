# GetFeedback MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/getfeedback)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage online surveys, track real-time responses, and oversee feedback data via AI agents with GetFeedback.

## Description
Connect your **GetFeedback** account to any AI agent to automate your customer feedback and survey reporting workflows through the Model Context Protocol (MCP). GetFeedback is a powerful, mobile-friendly survey platform that helps brands collect and analyze customer sentiment in real-time. This MCP server enables you to retrieve survey results, monitor completion statuses, and trigger survey invitations directly through natural conversation.

### Key Features

- **Survey Orchestration** — List all active surveys in your account and fetch detailed structural metadata for each form.
- **Real-time Response Tracking** — Retrieve customer feedback as it arrives, including detailed answer payloads and completion timestamps.
- **Advanced Filtering** — List survey responses filtered by status (started, completed) or created after a specific date for targeted reporting.
- **Automated Invitations** — Trigger survey emails to a list of recipients programmatically from your chat interface.
- **Identity Oversight** — Access global profile information for the authenticated GetFeedback user to ensure correct account context.
- **Data Connectivity** — Verify your API connection and account health to maintain seamless feedback loops.
- **Asynchronous Monitoring** — Fetch high-level response counts and status metrics to track survey performance instantly.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your GetFeedback Access Token (found in your Account Settings)
3. Start managing your customer feedback from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Experience (CX) Managers** — quickly check for new survey completions or fetch high-level sentiment summaries without manual exports.
- **Support Leads** — get a real-time overview of feedback associated with recent customer interactions via simple AI commands.
- **Marketing Analysts** — automate the retrieval of survey data for weekly reporting and brand health tracking.


## Available Tools (12)
- **check_api_limits**: Verify connectivity
- **verify_api_connection**: Check connection
- **get_my_identity**: Get user identity
- **get_response_details**: Get response metadata
- **get_survey_stats**: Get response count
- **get_survey_details**: Get survey metadata
- **list_completed_feedback**: Filter for completed
- **list_feedback_page**: Paginated responses
- **list_recent_feedback**: Filter by date
- **list_survey_responses**: List feedback data
- **list_surveys**: List all surveys
- **send_survey_invites**: Trigger survey email


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GetFeedback** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active surveys in my GetFeedback account."

**🤖 AI Agent:**
> Retrieving surveys... I found 4 active surveys, including 'Customer Satisfaction 2024' (ID: 12345) and 'Product Beta Feedback'. Which one would you like to see responses for?

---

**👤 You:**
> "Show me the last 5 completed responses for survey '12345'."

**🤖 AI Agent:**
> Fetching responses... For survey 12345, I found 5 recent completions. Most users are giving high ratings for 'Ease of Use', but some mentioned 'Pricing' as a concern.

---

**👤 You:**
> "Send the 'Onboarding Survey' (ID: 98765) to ['user1@test.com', 'user2@test.com']."

**🤖 AI Agent:**
> Invitations sent! I have successfully queued the survey invites for both recipients via GetFeedback. They should receive the emails shortly.


## ❓ FAQ

**Q: How do I get an Access Token for GetFeedback?**
Log in to GetFeedback, navigate to your account settings or profile, and look for the API section to generate your Personal Access Token.

**Q: Can I see incomplete survey responses?**
Yes! The 'list_survey_responses' tool allows you to filter by status. You can view responses that were 'started' but not yet finished, as well as 'completed' ones.

**Q: How do I send a survey to a list of people?**
Use the 'send_survey_invites' tool. Provide the Survey ID and a JSON array of email addresses to trigger the invitations instantly.

**Q: Is the data returned in real-time?**
Yes, all feedback data retrieved through this MCP server is fetched directly from the GetFeedback Reporting API, providing you with the latest available records.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/getfeedback](https://vinkius.com/mcp/getfeedback)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GetFeedback** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `getfeedback` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GetFeedback** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "getfeedback": {
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
