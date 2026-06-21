# Alchemer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/alchemer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Survey and feedback orchestration — manage surveys, responses, and reports via AI.

## Description
Connect your **Alchemer (formerly SurveyGizmo)** account to your AI agent to unlock professional survey management and customer feedback orchestration. From auditing survey structures and questions to retrieving real-time responses and generating granular reports, your agent handles your feedback lifecycle through natural conversation.

### What you can do

- **Survey Orchestration** — List and retrieve details for surveys, including their current status and technical metadata
- **Question Management** — List and audit survey questions to ensure your data collection is precisely configured
- **Response Auditing** — Retrieve and analyze individual or aggregated survey responses directly from chat
- **Reporting & Campaigns** — List and manage survey reports and campaigns to monitor your data distribution and analysis
- **Contact Oversight** — List and manage contact lists used for targeted survey distribution

### How it works

1. Subscribe to this server
2. Enter your Alchemer API Token, API Secret, and Region (US, EU, or CA)
3. Start managing your surveys and retrieving feedback insights through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Market Researchers** — automate survey audits and monitor response counts effortlessly
- **Customer Experience Leads** — quickly look up specific customer responses and identify sentiment trends
- **Product Managers** — research feature feedback and audit survey question flows on the fly
- **Data Analysts** — retrieve granular survey data for external analysis and reporting using simple commands


## Available Tools
- **list_surveys**: List account surveys
- **get_survey_details**: Get survey metadata
- **list_survey_questions**: List survey questions
- **get_question_details**: Get question metadata
- **list_survey_responses**: List survey submissions
- **get_response_details**: Get response data
- **list_survey_reports**: List survey reports
- **list_survey_campaigns**: List distribution campaigns
- **list_contact_lists**: List survey contacts
- **get_account_usage**: Check account status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Alchemer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active surveys in my Alchemer account."

**🤖 AI Agent:**
> I've retrieved your surveys. You have 8 active surveys, including '2026 Customer Satisfaction', 'Product Market Fit', and 'Event Feedback'. Would you like to see the response count for any of them?

---

**👤 You:**
> "Show me the last 5 responses for survey ID 1234567."

**🤖 AI Agent:**
> I've retrieved the latest 5 responses for survey 1234567. 4 are 'Complete' and 1 is 'Partial'. Would you like me to analyze the data for specific questions in these responses?

---

**👤 You:**
> "List all questions in the 'Customer Satisfaction' survey."

**🤖 AI Agent:**
> I've retrieved the question list for your Customer Satisfaction survey. It contains 15 questions, including 'Net Promoter Score (NPS)', 'Feature Rating', and 'Open Feedback'. Would you like to see the technical settings for the NPS question?


## ❓ FAQ

**Q: How do I find my Alchemer API Token and Secret?**
Log in to Alchemer as an admin, navigate to **Account** > **Integrations** > **API Access**. You can generate and copy your `api_token` and `api_token_secret` there.

**Q: Which region should I choose?**
Choose the region based on your account's data center: **US** (api.alchemer.com), **EU** (api.alchemer.eu), or **CA** (api.alchemer.ca).

**Q: Can I retrieve responses for a specific survey?**
Yes! Use the `list_survey_responses` tool and provide the Survey ID. Your agent will retrieve the latest submissions, including timestamps and completion status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alchemer](https://vinkius.com/mcp/alchemer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Alchemer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `alchemer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Alchemer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "alchemer": {
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
