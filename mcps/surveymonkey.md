# SurveyMonkey MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/surveymonkey)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage surveys, analyze responses, and automate feedback workflows directly through SurveyMonkey's API.

## Description
Connect your **SurveyMonkey** account to any AI agent to streamline your market research and data collection. This server allows you to interact with your surveys, pages, questions, and responses using natural language.

### What you can do

- **Survey Management** — List, create, retrieve, and update surveys within your account.
- **Structure Inspection** — Fetch the complete structure of a survey, including all pages and questions, to understand the flow.
- **Response Analysis** — Retrieve individual or bulk responses to analyze feedback and trends instantly.
- **Collector Control** — Manage distribution channels (collectors) to track how and where your surveys are being shared.
- **Content Creation** — Programmatically add pages and questions to existing surveys to build complex forms dynamically.

### How it works

1. Subscribe to this server
2. Enter your SurveyMonkey Access Token from the Developer Portal
3. Start managing your surveys from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Market Researchers** — quickly pull response data for analysis without manual exports.
- **Product Managers** — monitor customer feedback and feature requests in real-time.
- **Marketing Teams** — automate the creation and distribution of campaign surveys.


## Available Tools (17)
- **create_survey_collector**: g., Web Link, Email).

Create a new collector
- **create_survey_page**: Add a page to a survey
- **create_survey_question**: Create a question
- **create_survey**: Provide the survey configuration as a JSON payload.

Create a new survey
- **delete_survey**: Delete a survey
- **get_collector**: Retrieve collector details
- **get_response**: Retrieve a specific response
- **get_survey_details**: Get full survey structure (pages, questions)
- **get_survey_page**: Retrieve a specific page
- **get_survey**: Retrieve details for a specific survey
- **list_survey_collectors**: List collectors for a survey
- **list_survey_pages**: List pages in a survey
- **list_survey_questions**: List questions on a page
- **list_survey_responses_bulk**: Retrieve full response data for multiple respondents
- **list_survey_responses**: List responses for a survey
- **list_surveys**: List all surveys for the authenticated user
- **update_survey**: Provide the fields to update as a JSON payload.

Update survey details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SurveyMonkey** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my surveys in SurveyMonkey."

**🤖 AI Agent:**
> I've retrieved your surveys. You have 3 active surveys: 'Customer Satisfaction 2024' (ID: 401234), 'Product Feedback' (ID: 401235), and 'Employee Engagement' (ID: 401236).

---

**👤 You:**
> "Show me the full structure and questions for survey 401234."

**🤖 AI Agent:**
> Fetching details for survey 401234... This survey has 2 pages. Page 1 contains 3 questions (Multiple Choice and Text), and Page 2 contains a Rating Scale question. Would you like to see the specific question texts?

---

**👤 You:**
> "Get the latest bulk responses for survey 401235."

**🤖 AI Agent:**
> I've pulled the latest bulk responses for survey 401235. I found 50 recent responses. Most respondents rated the product 'Very Satisfied'. Would you like a summary of the open-ended comments?


## ❓ FAQ

**Q: Can I retrieve the entire structure of a survey including all its questions at once?**
Yes. Use the `get_survey_details` tool with the specific Survey ID. It will return the full hierarchy of pages and questions configured for that survey.

**Q: Is it possible to export or list all responses for a survey in bulk?**
Absolutely. The `list_survey_responses_bulk` tool allows you to fetch multiple responses at once, making it ideal for data analysis and reporting.

**Q: Can I see how my survey is being distributed?**
Yes. You can use `list_survey_collectors` to see all active distribution channels (links, emails, etc.) associated with a specific survey.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/surveymonkey](https://vinkius.com/mcp/surveymonkey)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SurveyMonkey** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surveymonkey` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SurveyMonkey** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surveymonkey": {
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
