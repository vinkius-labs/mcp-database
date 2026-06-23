# Nicereply MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nicereply)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Measure customer satisfaction via Nicereply — track survey responses, ratings, and stats directly from your AI agent.

## Description
Connect your **Nicereply** account to your AI agent and gain deep insights into your customer satisfaction and agent performance through natural conversation.

### What you can do

- **Response Monitoring** — List and inspect all customer satisfaction ratings and feedback responses in real-time.
- **Survey Analytics** — Access CSAT, CES, and NPS surveys and retrieve detailed performance metrics and statistics.
- **Agent Performance** — List workspace users and monitor their individual ratings and feedback scores.
- **Customer Insights** — View customer profiles and their historical feedback patterns.
- **Rating Standards** — Retrieve the definitions of rating values and scales used across your surveys.
- **Deep Inspection** — Fetch complete metadata for specific responses or surveys using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your Nicereply API Key (Private Key)
3. Start monitoring customer satisfaction from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Success Managers** — quickly check for negative feedback or overall survey performance without opening the dashboard.
- **Support Leads** — monitor agent ratings and satisfaction trends during daily standups.
- **Product Teams** — analyze customer sentiment and feedback regarding specific features or releases.


## Available Tools (10)
- **get_customer**: Get specific customer details
- **get_me**: Get current user details
- **get_rating_values**: List possible rating values
- **get_response**: Get specific response details
- **get_survey_stats**: Get survey statistics
- **get_survey**: Get specific survey details
- **list_customers**: List Nicereply customers
- **list_responses**: List feedback responses
- **list_surveys**: List all surveys
- **list_users**: List workspace users (agents)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nicereply** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the latest customer feedback responses."

**🤖 AI Agent:**
> I've retrieved the recent responses. You have 5 new ratings: 4 'Great' and 1 'Neutral'. The neutral feedback mentioned 'Slow response time' from a ticket yesterday. Would you like the full details for that response?

---

**👤 You:**
> "What is the current performance of our CSAT survey?"

**🤖 AI Agent:**
> Fetching CSAT survey stats... Your current CSAT score is 92%, based on 156 responses this month. This is a 2% increase compared to last month. Shall I provide a breakdown of the scores?

---

**👤 You:**
> "List all active surveys in my Nicereply account."

**🤖 AI Agent:**
> Retrieving surveys... You have 3 active surveys: 'Post-Ticket CSAT' (ID: srv_123), 'Product Feedback NPS' (ID: srv_456), and 'Onboarding CES'. Which one would you like more information about?


## ❓ FAQ

**Q: Where do I find my Nicereply API Key?**
Log in to Nicereply, go to Settings > API and Integrations, and you will find your 'Private API Key' there.

**Q: Does this support NPS surveys?**
Yes! Nicereply supports CSAT, CES, and NPS. You can list all your surveys using the `list_surveys` tool and get stats for any of them.

**Q: Can I see feedback for a specific support agent?**
You can use the `list_users` tool to find the Agent ID and then filter responses or view individual ratings recorded in the platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nicereply](https://vinkius.com/mcp/nicereply)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nicereply** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nicereply` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nicereply** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nicereply": {
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
