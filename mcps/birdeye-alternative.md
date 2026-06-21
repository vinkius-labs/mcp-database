# Birdeye MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/birdeye-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Grow your local business reputation with review management, customer surveys, and listings that drive more foot traffic.

## Description
Connect your **Birdeye** account to any AI agent and take full control of your online reputation management and customer experience workflows through natural conversation.

### What you can do

- **Review Orchestration** — List and manage customer reviews across multiple platforms (Google, Facebook, etc.) programmatically, retrieving detailed high-fidelity comments and ratings in real-time
- **Automated Check-ins** — Programmatically trigger review requests (check-ins) via SMS or Email to coordinate high-fidelity feedback collection from your recent visitors
- **Sentiment Intelligence** — Access complete customer profiles and retrieve detailed sentiment history to maintain a perfectly coordinated overview of your brand health
- **Survey & Feedback Architecture** — Programmatically dispatch custom surveys to specific customers and monitor their high-fidelity responses directly through your agent
- **Multi-Location Visibility** — Retrieve complete directories of all your business branches and locations to coordinate your organizational reputation programmatically

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** and **Business ID (bid)** from your Birdeye dashboard (Settings > Integrations > API)
3. Start managing your customer experience from Claude, Cursor, or any MCP client

No more manual logging into individual review sites or missing critical feedback. Your AI acts as your dedicated reputation manager and customer success coordinator.

### Who is this for?

- **Marketing Managers** — instantly retrieve high-level review summaries and monitor brand sentiment using natural language commands
- **Customer Success Teams** — automate the dispatch of review requests and track customer satisfaction without leaving your workspace
- **Multi-Location Owners** — monitor reputation performance across all branches and coordinate surveys through simple AI queries


## Available Tools
- **customer_checkin**: Trigger a review request (Check-in)
- **create_customer**: Add a new customer profile
- **get_customer_details**: Get full customer profile
- **list_business_locations**: List all business locations
- **list_reviews**: List customer reviews
- **trigger_survey**: Send a custom survey to a customer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Birdeye** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the latest 5-star reviews for my business in Birdeye."

**🤖 AI Agent:**
> I've retrieved your top reviews. You recently received 10 new 5-star ratings across Google and Facebook. Highlights include high praise for your 'Fast Response Time'. Would you like to see the detailed metadata for these?

---

**👤 You:**
> "Send a review request to 'John Smith' (john@example.com)."

**🤖 AI Agent:**
> Customer check-in complete! I've successfully triggered a review request for John Smith. He will receive an automated notification shortly. Shall I monitor the status for any response?

---

**👤 You:**
> "Show the sentiment profile for customer ID '12345'."

**🤖 AI Agent:**
> Accessing customer intelligence... John Doe (ID: 12345) has a consistently 'Positive' sentiment profile across 3 reviews and 1 survey response. His latest NPS score was 10. Need more historical context from his high-fidelity profile?


## ❓ FAQ

**Q: How do I find my Birdeye API Key and Business ID?**
Log in to your account, navigate to **Settings** > **Integrations** > **API**, and you will find your API Key and the Business ID (bid).

**Q: Can I request a review via AI?**
Yes! The `customer_checkin` tool allows your agent to record a customer visit and automatically send a review request via their preferred channel.

**Q: How do I check review ratings programmatically?**
Use the `list_reviews` tool and provide an optional `rating` filter (1-5) to retrieve specific categories of feedback directly from the platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/birdeye-alternative](https://vinkius.com/mcp/birdeye-alternative)
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
3. Set Type to "SSE", enter `birdeye-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Birdeye** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "birdeye-alternative": {
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
