# TrueReview MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/truereview)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Collect authentic customer reviews with automated requests and showcase testimonials that build trust and drive conversions.

## Description
Connect your **TrueReview** reputation management account to any AI agent and simplify how you collect customer feedback, manage review requests, and monitor your business rating through natural conversation.

### What you can do

- **Contact Management** — List and create customer records specifically for review and feedback targeting.
- **Review Requests** — Trigger instant review requests via SMS or Email for your customers directly via AI commands.
- **Campaign Tracking** — List available drip campaigns and review sequences to manage your outreach strategy.
- **Performance Reporting** — Retrieve summary reports of your review performance and feedback metrics to measure customer satisfaction.
- **Location Oversight** — List and manage business locations to ensure consistent reputation management across your organization.
- **Contact Insights** — Fetch detailed metadata and history for individual customer contacts.

### How it works

1. Subscribe to this server
2. Enter your TrueReview API Key and Location SID
3. Start managing your online reputation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Business Owners & Operators** — quickly trigger review requests for recent customers via simple AI commands.
- **Reputation Managers** — monitor feedback reports and verify campaign statuses across multiple locations.
- **Customer Success Teams** — manage contact lists and track review performance metrics directly from the workspace.


## Available Tools
- **create_contact**: Create a new customer contact
- **get_contact**: Get details for a specific contact
- **get_report_summary**: Get a summary report of reviews
- **list_campaigns**: List all review campaigns
- **list_contacts**: List all contacts for the location
- **list_locations**: List all business locations
- **send_review_request**: Send a review request to a customer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TrueReview** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all contacts in my TrueReview account."

**🤖 AI Agent:**
> I've retrieved your contacts. You have 25 active customer records including 'John Miller', 'Sarah Smith', and 'Robert Chen'. Would you like to send a review request to any of them?

---

**👤 You:**
> "Send an email review request to 'John Miller' (ID: 10293)."

**🤖 AI Agent:**
> Request sent! I've triggered the email review request for John Miller (ID: 10293). He should receive the link in his inbox shortly. I'll monitor for any updates.

---

**👤 You:**
> "Show me a summary of my recent reviews."

**🤖 AI Agent:**
> I've fetched your report summary. Over the last 30 days, you've received 12 new reviews with an average rating of 4.8 stars. Your response rate is currently 92%. Shall I list the individual feedback comments?


## ❓ FAQ

**Q: Can I send a review request via SMS using the AI?**
Yes! Use the `send_review_request` tool. Provide the Contact ID and set the type to 'sms'. The agent will trigger the SMS request through TrueReview instantly.

**Q: How do I see the overall feedback summary for my business?**
Run the `get_report_summary` query. The agent will retrieve a concise report of your review performance and customer satisfaction metrics.

**Q: Is it possible to add a new customer contact via AI?**
Absolutely. Use the `create_contact` action. Provide the first name, last name, and email or phone number to register a new customer for future review requests.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/truereview](https://vinkius.com/mcp/truereview)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TrueReview** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `truereview` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TrueReview** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "truereview": {
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
