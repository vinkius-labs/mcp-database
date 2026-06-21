# QuestionPro MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/questionpro)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/questionpro-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/questionpro-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Deploy AI to analyze survey responses, manage questionnaires, and extract actionable insights instantly.

## Description
Bring advanced survey analytics into your AI workflow with QuestionPro. Your agents can orchestrate end-to-end feedback loops by filtering folders for active campaigns, compiling real-time response statistics, retrieving granular participant data, and maintaining contact lists—all executed conversationally.

### What you can do
- Create, retrieve, and organize surveys with folder filtering
- Analyze real-time survey statistics and completion rates
- Collect and inspect individual respondent data
- Manage question banks and user administration
- Organize email outreach lists efficiently

### How it works
1. Log in to your QuestionPro account
2. Go to Integrations to generate your unique API key
3. Link the key in Vinkius to enable AI-powered survey management

### Who is it for?
Ideal for market researchers, HR teams, and product managers needing fast, AI-driven insights from customer and employee feedback.


## Available Tools
- **check_questionpro_status**: Verify connectivity
- **create_survey**: Create a survey
- **get_question**: Get question details
- **get_response**: Get response details
- **get_survey_stats**: Get survey statistics
- **get_survey**: Get survey details
- **list_surveys_by_folder**: List surveys by folder
- **list_email_lists**: List email lists
- **list_folders**: List folders
- **list_questions**: List survey questions
- **list_responses**: List survey responses
- **list_surveys**: List surveys
- **list_users**: List account users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **QuestionPro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show response rate and completion stats for our customer satisfaction survey"

**🤖 AI Agent:**
> The Customer Satisfaction Survey has a 65% response rate and an 82% completion rate so far. Would you like to see a breakdown by demographic?

---

**👤 You:**
> "Show me all active surveys with their response rates and completion percentages."

**🤖 AI Agent:**
> 9 active surveys. "Customer Experience 2025" leads with 3,421 responses (78% completion rate). "Employee Pulse Check" has 234 of 300 expected responses (78%). "Product Feature Priority" collected 1,890 responses with 82% completion. "Market Research Q2" at 567 responses but only 54% completion, suggesting friction in the form. "NPS Quarterly" scored 71 with 2,100 respondents. Total responses this quarter: 12,450. 3 surveys have response rates below 60%.

---

**👤 You:**
> "Export the detailed analytics report for the Customer Experience 2025 survey."

**🤖 AI Agent:**
> Analytics report generated for "Customer Experience 2025". Total responses: 3,421. Overall satisfaction: 4.3/5. Key findings: Product quality rated highest (4.6/5), pricing perceived as competitive by 72% of respondents, support response time is the top improvement area (mentioned 890 times). Demographics: 55% enterprise, 30% mid-market, 15% SMB. Trends vs last quarter: satisfaction up 0.3 points, NPS improved from 67 to 72. Report exported in PDF and Excel formats.


## Installation & Usage

To install and use the **QuestionPro** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/questionpro](https://vinkius.com/mcp/questionpro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
