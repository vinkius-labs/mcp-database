# KnoCommerce MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/knocommerce)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Analyze post-purchase surveys — list responses, audit customer feedback, and track attribution channels.

## Description
Connect your **KnoCommerce** data to your AI agent to unlock deep insights from your post-purchase surveys.

### Key Features

- **Survey Analysis** — List and audit all active surveys to understand your feedback collection strategy
- **Response Auditing** — Drill down into individual customer responses to see exactly what your buyers are saying
- **Customer Profiles** — View feedback history associated with specific customer IDs to build a complete buyer profile
- **Attribution Reporting** — Access aggregated channel attribution data to see which marketing efforts are actually working
- **Template Discovery** — Browse available survey templates to quickly launch new feedback campaigns

### Simple Setup

1. Get your API Key from the KnoCommerce dashboard
2. Configure the MCP server in your favorite client (Claude, Cursor, etc.)
3. Start querying your survey data using natural language


## Available Tools (10)
- **list_survey_responses**: You can optionally filter by survey_id to see feedback from a specific post-purchase interaction.

List responses for surveys
- **get_response_details**: Get details for a specific customer response
- **list_knocommerce_customers**: Useful for correlating feedback with specific buyer profiles.

List customers associated with survey data
- **get_customer_feedback_profile**: Get details for a specific customer feedback profile
- **list_survey_questions**: Use this to understand the data structure of the responses.

List all questions in a specific survey
- **get_channel_attribution_report**: This is essential for understanding which marketing channels are driving customer acquisition.

Get the latest channel attribution report
- **list_survey_templates**: List available survey templates
- **check_knocommerce_api_status**: Check the status of the KnoCommerce API integration
- **list_surveys**: Use this to identify survey IDs for analyzing specific campaigns or response sets.

List all KnoCommerce surveys
- **get_survey_details**: Returns survey title, status, and high-level configuration.

Get details for a specific survey


## 💬 Prompt Examples

Here are some examples of how you can interact with the **KnoCommerce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active surveys in my KnoCommerce account"

**🤖 AI Agent:**
> I've found 3 active surveys: 'Post-Purchase General', 'Holiday Special Feedback', and 'Product Fit Research'. Which one would you like to examine?

---

**👤 You:**
> "Show me the latest responses for survey 'kc_123'"

**🤖 AI Agent:**
> Retrieving responses for 'kc_123'… I've found 15 recent submissions. The overall sentiment seems positive, with most users mentioning 'Fast Shipping' as the primary reason for purchase.

---

**👤 You:**
> "Give me a channel attribution report"

**🤖 AI Agent:**
> The attribution report shows that 45% of your customers found you via 'Instagram Ads', 20% through 'Direct Search', and 15% from 'Email Marketing'.


## ❓ FAQ

**Q: Where do I find my KnoCommerce API Key?**
Log in to your KnoCommerce dashboard and navigate to **Settings** > **API Keys**. You can generate a new REST API key there.

**Q: Can I see the individual questions of a survey?**
Yes, use the `list_survey_questions` tool with the specific `survey_id` to retrieve all questions and their configuration.

**Q: Does this support creating new surveys?**
The current version focus on data retrieval and analysis. You can list templates, but survey creation should be done in the KnoCommerce dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/knocommerce](https://vinkius.com/mcp/knocommerce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **KnoCommerce** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `knocommerce` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **KnoCommerce** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "knocommerce": {
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
