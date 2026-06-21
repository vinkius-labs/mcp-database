# Porsline MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/porsline)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Automate surveys and feedback via Porsline — manage surveys, responses, and reports directly from any AI agent.

## Description
Connect your **Porsline** account to any AI agent and simplify your survey creation, response tracking, and feedback orchestration through natural conversation.

### What you can do

- **Survey Management** — List all surveys, retrieve detailed metadata, status, and summary for each form
- **Response Tracking** — Access individual responses and answers to stay on top of your user feedback
- **Live Reporting** — Query aggregate metrics and summary reports for any survey to understand performance
- **Folder Coordination** — List organizational folders to manage your survey distribution and project structure
- **Direct Insights** — Monitor your survey pipeline and engagement metrics directly from your agent

### How it works

1. Subscribe to this server
2. Enter your Porsline API Token from your account settings
3. Start managing your surveys from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **create_survey**: Create a survey
- **duplicate_survey**: Duplicate a survey
- **export_responses**: Export responses
- **get_report**: Get survey report
- **get_response**: Get response details
- **get_survey**: Get survey details
- **list_folders**: List folders
- **list_questions**: List questions
- **list_responses**: List responses
- **list_surveys**: List surveys
- **check_porsline_status**: Verify connectivity
- **create_folder**: Create a folder


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Porsline** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my surveys in Porsline."

**🤖 AI Agent:**
> I've retrieved your surveys. You have 5 active surveys, including 'Customer Satisfaction 2024' and 'Product Feedback'.

---

**👤 You:**
> "Show me all active surveys and their response rates for the current quarter."

**🤖 AI Agent:**
> You have 7 active surveys this quarter. "Customer Satisfaction Q2" has 1,247 responses (62% completion rate, NPS score: 72). "Employee Engagement" collected 89 of 120 expected responses (74%). "Product Feedback v3" has 456 completions with an average time of 4.2 minutes. "Event Registration" is your newest with 34 entries. Total responses this quarter: 2,891 across all surveys. 2 surveys have response rates below 50% and may need reminder emails.

---

**👤 You:**
> "Get the detailed results and analytics for the Customer Satisfaction Q2 survey."

**🤖 AI Agent:**
> Customer Satisfaction Q2 detailed results. 1,247 total responses. NPS: 72 (Promoters: 68%, Passives: 18%, Detractors: 14%). Satisfaction by category: Product quality 4.5/5, Customer support 4.3/5, Value for money 4.1/5, Ease of use 4.6/5. Top requested improvement: "Faster response times" (mentioned 234 times). 89% would recommend to a colleague. Response trend: 12% increase vs Q1. Average completion time: 3.8 minutes.


## ❓ FAQ

**Q: Can I list all my active surveys using my AI agent?**
Yes! Use the `list_surveys` tool to retrieve a comprehensive list of all surveys registered in your Porsline account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/porsline](https://vinkius.com/mcp/porsline)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Porsline** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `porsline` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Porsline** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "porsline": {
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
