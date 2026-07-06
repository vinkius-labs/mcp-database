# Wenjuanxing / 问卷星 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wenjuanxing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Leading online survey and form platform in China — manage questionnaires, responses, and reports via AI.

## Description
Empower your AI agent to orchestrate your data collection and research with **Wenjuanxing** (WJX), the premier online survey platform in China. By connecting Wenjuanxing to your agent, you transform complex questionnaire management, response auditing, and data analysis into a natural conversation. Your agent can instantly list your surveys, retrieve detailed structure and metadata, monitor real-time response counts, and even generate high-level analysis reports without you ever needing to navigate the comprehensive web interface. Whether you are conducting market research or auditing employee engagement, your agent acts as a real-time research assistant, keeping your data accurate and your insights moving.

### What you can do

- **Survey Orchestration** — List all questionnaires and retrieve detailed structure and metadata for each.
- **Response Monitoring** — List and retrieve actual response data to monitor participation and engagement.
- **Analytical Reporting** — Retrieve high-level summary reports and quantitative statistics for survey results.
- **Content Control** — Create new survey structures and update the status of existing questionnaires.
- **Organization Insights** — Browse survey folders and retrieve metadata about your Wenjuanxing account.

### How it works

1. Subscribe to this server
2. Enter your Wenjuanxing App ID and App Key
3. Start managing your research and surveys through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Market Researchers** — monitor survey progress and audit qualitative data through natural language queries.
- **HR Managers** — manage employee feedback surveys and monitor response rates directly from your AI-powered workspace.
- **Marketing Leads** — coordinate customer satisfaction research and retrieve summary statistics via a unified AI interface.
- **Wenjuanxing Power Users** — integrate your existing research workflows into your AI-driven daily routines.


## Available Tools (10)
- **list_groups**: List survey groups
- **list_responses**: List survey responses
- **list_surveys**: List questionnaires
- **query_surveys**: Search questionnaires by keyword
- **update_survey_status**: g., publish, pause) of a specific survey.

Update survey status
- **create_survey**: Create a new questionnaire
- **get_account_info**: Get user account metadata
- **get_report**: Get survey summary report
- **get_stats**: Get survey statistics
- **get_survey**: Get questionnaire details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wenjuanxing / 问卷星** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active surveys in my Wenjuanxing account."

**🤖 AI Agent:**
> I've retrieved your questionnaires. You have 8 active surveys, including 'Customer Satisfaction 2026' and 'Product Feedback - V2'. Would you like to check the response count for any of them?

---

**👤 You:**
> "Show me the responses for survey activity '8821'."

**🤖 AI Agent:**
> I've retrieved the responses for survey 8821. There are 150 completed submissions. Would you like to see the details of the most recent ones or generate a summary report?

---

**👤 You:**
> "What are the statistics for questionnaire '9920'?"

**🤖 AI Agent:**
> I've retrieved the quantitative statistics for survey 9920. For question 1, 65% of respondents selected 'Highly Satisfied'. For question 2, the average rating is 4.2/5.0. Should I retrieve the full report?


## ❓ FAQ

**Q: How do I find my Wenjuanxing App ID and Key?**
Log in to your Wenjuanxing account (Enterprise/Flagship version), go to the Open API Platform (openapi.wjx.cn) or check the 'API/SSO' section in your user settings to find your App ID and Key.

**Q: Can I see quantitative statistics for survey questions?**
Yes. Use the `get_stats` tool with your activity ID to retrieve counts and percentages for each answer option in your survey.

**Q: Is it possible to search questionnaires by keyword?**
Yes! You can use the `query_surveys` tool to find specific questionnaires in your account based on their title or activity keyword.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wenjuanxing](https://vinkius.com/mcp/wenjuanxing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wenjuanxing / 问卷星** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wenjuanxing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wenjuanxing / 问卷星** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wenjuanxing": {
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
