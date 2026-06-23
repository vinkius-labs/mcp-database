# Birdeye MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/birdeye)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage reputation and customer experience via Birdeye — list reviews, manage contacts, and trigger surveys directly from any AI agent.

## Description
Connect your **Birdeye** account to any AI agent and orchestrate your customer experience and reputation management workflows through natural conversation.

### What you can do

- **Review Management** — List and retrieve detailed customer reviews and fetch review summaries by source.
- **Customer Interaction** — Reply to reviews directly from the agent to maintain high engagement.
- **CX Automation** — Trigger customer check-ins to automatically send review or survey requests.
- **Survey Insights** — List available surveys and retrieve customer responses for analysis.
- **Contact Oversight** — Manage your business contacts and retrieve detailed profile information.
- **Location Tracking** — Access and list all business locations managed within your account.

### How it works

1. Subscribe to this server
2. Enter your Birdeye API Key and Business ID
3. Start managing your reputation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Reputation Managers** — quickly check and respond to reviews without navigating multiple dashboards.
- **Customer Success Teams** — monitor survey results and contact details straight from their workflow tools.
- **Marketing Leads** — retrieve review summaries and location data for reporting.


## Available Tools (10)
- **checkin_customer**: Check-in a customer to trigger review/survey requests
- **get_business_info**: Retrieve core business information
- **get_contact**: Get specific contact details
- **get_review_summary**: Get a summary of review counts by source
- **get_survey_responses**: Get responses for a specific survey
- **list_contacts**: List customer contacts
- **list_locations**: List all business locations
- **list_reviews**: List customer reviews
- **list_surveys**: List all surveys
- **reply_to_review**: Reply to a specific customer review


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Birdeye** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 reviews received on Birdeye."

**🤖 AI Agent:**
> I've retrieved your recent reviews. You have 5 new entries, including a 5-star review from Alice Johnson on Google and a 4-star review on Facebook. Would you like to reply to any of them?

---

**👤 You:**
> "Check in a customer: John Doe, john@example.com."

**🤖 AI Agent:**
> Customer 'John Doe' has been checked in successfully. Birdeye will now send the automated review request according to your settings.

---

**👤 You:**
> "Show my survey responses for survey surv_123."

**🤖 AI Agent:**
> Retrieving responses for survey surv_123... I found 3 recent responses. Most customers mentioned 'Excellent service' and 'Fast delivery'. Should I summarize the full feedback?


## ❓ FAQ

**Q: Can I reply to a review using the agent?**
Yes! Use the `reply_to_review` tool with the Review ID and your message. If the source allows API replies, your message will be posted to Birdeye instantly.

**Q: How do I see the average rating for my business?**
Simply ask the agent to `get_review_summary`. It will retrieve the overall counts and ratings aggregated across all supported platforms (Google, Facebook, etc.).

**Q: Can I trigger a review request for a specific customer?**
Yes. Use the `checkin_customer` action with the customer's name and email. This will trigger the automated review and survey sequence configured in your Birdeye account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/birdeye](https://vinkius.com/mcp/birdeye)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Birdeye** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `birdeye` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Birdeye** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "birdeye": {
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
