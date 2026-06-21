# OneLocal LocalReviews MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/onelocal-localreviews)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Boost your local business visibility with automated review collection, reputation monitoring, and response management tools.

## Description
Connect your **OneLocal LocalReviews** account to any AI agent and take full control of your online reputation management and automated review orchestration through natural conversation.

### What you can do

- **Review Portfolio Orchestration** â€” List and manage all received customer reviews programmatically, retrieving detailed sentiment metadata and star ratings
- **Request & Campaign Intelligence** â€” Programmatically trigger and monitor review request campaigns to maintain a perfectly coordinated feedback pipeline
- **Reputation Architecture Monitoring** â€” Access real-time status updates for new reviews and track organizational rating trends directly through your agent
- **Metadata Management** â€” Programmatically retrieve customer identifiers and response history to maintain a perfectly coordinated audit trail
- **Operational Monitoring** â€” Verify account-level API connectivity and monitor submission volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your OneLocal dashboard (Settings > API)
3. Start orchestrating your local growth from Claude, Cursor, or any MCP client

No more manual following up for reviews or missing critical negative feedback. Your AI acts as your dedicated reputation coordinator and review architect.

### Who is this for?

- **Business Owners** â€” instantly retrieve review summaries and monitor reputation health using natural language commands
- **Marketing Managers** â€” verify individual review metadata and track campaign results without leaving your creative workspace
- **Developers** â€” integrate high-speed OneLocal review data into custom dashboards and reporting tools through simple AI queries


## Available Tools (10)
- **check_onelocal_status**: Verify OneLocal API connectivity
- **get_campaign**: Get campaign details
- **get_location**: Get location details
- **get_reputation**: Get reputation overview
- **get_review**: Get review details
- **list_campaigns**: List all campaigns
- **list_locations**: List all locations
- **list_referrals**: List all referrals
- **list_reviews**: List all reviews
- **request_review**: Request a review


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OneLocal LocalReviews** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all recent reviews for my business."

**🤖 AI Agent:**
> You have 24 reviews this month. Average rating: 4.7/5. 3 reviews need a response. The latest is a 5-star review on Google from Lisa Chen. Would you like to respond?

---

**👤 You:**
> "Send a review request to john@example.com."

**🤖 AI Agent:**
> Review request sent to john@example.com. The email includes links to Google and Facebook review pages. I'll track the response. Would you like to send more requests?

---

**👤 You:**
> "Show my overall reputation score."

**🤖 AI Agent:**
> Your reputation score is 4.6/5 across 3 platforms. Google: 4.7 (180 reviews), Facebook: 4.5 (45 reviews), Yelp: 4.4 (22 reviews). Trend: +0.2 this quarter. Would you like to see review sentiment analysis?


## ❓ FAQ

**Q: How do I send a review request to a customer?**
Use the `request_review` tool with the customer's email address and optional name. The request is sent immediately through your OneLocal account.

**Q: Can I monitor my overall reputation score?**
Yes. Use `get_reputation` to retrieve your aggregate reputation score with review trends, sentiment analysis, and platform-by-platform breakdown.

**Q: How do I track referral performance?**
Use `list_referrals` to see all customer referrals with their source, status, and conversion tracking data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/onelocal-localreviews](https://vinkius.com/mcp/onelocal-localreviews)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OneLocal LocalReviews** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `onelocal-localreviews` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OneLocal LocalReviews** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "onelocal-localreviews": {
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
