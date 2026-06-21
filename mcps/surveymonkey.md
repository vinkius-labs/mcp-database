# SurveyMonkey MCP Server

Manage surveys, analyze responses, and automate feedback workflows directly through SurveyMonkey's API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/surveymonkey)

## Overview
**Category:** marketing-automation
**Tools Count:** 17

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


## Available Tools
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


## Installation & Usage

To install and use the **SurveyMonkey** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/surveymonkey](https://vinkius.com/mcp/surveymonkey)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
