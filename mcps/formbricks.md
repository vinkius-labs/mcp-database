# Formbricks MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/formbricks)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/formbricks-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/formbricks-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage surveys, capture feedback, and oversee experience management via AI agents with Formbricks.

## Description
Connect your **Formbricks** account to any AI agent to automate your survey management and customer experience workflows through the Model Context Protocol (MCP). Formbricks is the open-source alternative to Typeform and Qualtrics, designed to help you capture feedback at every stage of the user journey. This MCP server enables you to manage your surveys, retrieve responses, and organize contacts directly through natural conversation.

### Key Features

- **Survey Control** — List all surveys in your environment, fetch detailed question metadata, and create or update surveys instantly.
- **Feedback Management** — Retrieve real-time survey responses and fetch specific details for individual submissions to understand user sentiment.
- **Contact Oversight** — Access your CRM contacts (People), search for specific members, and retrieve complete metadata profiles.
- **Categorization** — List and manage organization tags to keep your surveys and feedback loops well-organized.
- **System Metadata** — Fetch environment and product information to maintain full context of your Formbricks setup.
- **Operational Efficiency** — Delete surveys or update statuses (draft/published) directly through simple AI commands.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Formbricks Personal API Key (found in Settings > API Keys)
3. Start managing your feedback and experience data from Claude, Cursor, or any MCP client

### Who is this for?

- **Product Managers** — quickly check feedback on a new feature or list responses from a targeted survey.
- **Customer Success Teams** — automate the retrieval of contact details and sentiment data from survey submissions.
- **Marketing Operations** — manage survey lifecycles and organize feedback loops via simple AI commands.


## Available Tools
- **create_survey**: Create a new survey
- **delete_survey**: Remove a survey
- **get_environment_info**: Get environment details
- **get_contact_details**: Get contact metadata
- **get_product_info**: Get product details
- **get_response**: Get response details
- **get_survey**: Get survey details
- **list_contacts**: List CRM contacts
- **list_responses**: List survey responses
- **list_surveys**: List all surveys
- **list_tags**: List organization tags
- **update_survey**: Update survey settings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Formbricks** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active surveys in my Formbricks account."

**🤖 AI Agent:**
> Retrieving surveys... I found 4 surveys, including 'Feature Request' (published) and 'Post-Onboarding Survey' (published). Would you like to see the responses for any of these?

---

**👤 You:**
> "Show me the last 5 responses for survey ID 'sur_abc123'."

**🤖 AI Agent:**
> Fetching responses... For survey sur_abc123, I found 5 recent submissions. Sentiment appears generally positive with key requests for 'Dark Mode' and 'API improvements'.

---

**👤 You:**
> "Find the contact profile for 'john.doe@example.com'."

**🤖 AI Agent:**
> Searching contacts... I found a profile for John Doe. He has submitted 3 survey responses and is tagged with 'Beta User'.


## Installation & Usage

To install and use the **Formbricks** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/formbricks](https://vinkius.com/mcp/formbricks)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
