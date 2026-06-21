# GatherUp MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gatherup)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage customer reviews, track feedback, and automate review requests via AI agents with GatherUp.

## Description
Connect your **GatherUp** account to any AI agent to automate your review management and customer feedback workflows through the Model Context Protocol (MCP). GatherUp is a powerful platform that helps businesses monitor reputation, collect 1st-party feedback, and showcase 3rd-party reviews from sites like Google and Facebook. This MCP server enables you to track review streams, reply to customers, and trigger automated review requests directly through natural conversation.

### Key Features

- **Business Unit Oversight** — List all business locations and retrieve high-level configuration metadata for each unit.
- **Feedback Management** — Access and retrieve first-party feedback left directly by customers via your GatherUp surveys.
- **Online Review Tracking** — Monitor third-party reviews from Google, Facebook, Yelp, and more in a centralized feed.
- **Real-time Interaction** — Send replies to both internal feedback and supported external reviews directly from your chat interface.
- **Review Request Automation** — Trigger new review invites (email/SMS) to specific customers to boost your reputation.
- **Contact Management** — Add and sync customer profiles to specific business locations programmatically.
- **Reputation Metrics** — Fetch high-level statistics and sentiment analysis for any business location instantly.
- **API Health Monitoring** — Verify your connection to the GatherUp v2 API environment seamlessly.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your GatherUp Client ID and API Token (found in Settings > API)
3. Start managing your reputation from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing Managers** — quickly check recent ratings or reply to negative feedback without manual dashboard navigation.
- **Customer Success Teams** — get a real-time overview of customer sentiment across all locations via simple AI commands.
- **Operations Teams** — automate the sending of review requests and verify customer synchronization seamlessly.


## Available Tools
- **add_new_customer**: Sync a customer
- **verify_api_connection**: Check connection
- **get_review_metrics**: Get location stats
- **get_account_info**: Get user identity
- **list_business_locations**: List business units
- **list_customer_contacts**: List customers
- **list_internal_feedback**: List direct feedback
- **list_online_reviews**: List external reviews
- **reply_to_feedback**: Reply to internal feedback
- **reply_to_online_review**: g. Google or Facebook).

Reply to external review
- **search_all_reviews**: Search all feedback
- **send_review_invite**: Request a review


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GatherUp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my business locations in GatherUp."

**🤖 AI Agent:**
> Retrieving businesses... I found 3 locations: 'Downtown Cafe' (ID: biz_123), 'Westside Bistro' (ID: biz_456), and 'Airport Lounge'. Which one would you like to check reviews for?

---

**👤 You:**
> "Show me the 5 most recent Google reviews for 'Downtown Cafe' (ID: biz_123)."

**🤖 AI Agent:**
> Fetching reviews... For Downtown Cafe, I found 5 recent Google reviews. You have four 5-star ratings and one 3-star rating mentioning 'long wait times'. Would you like to draft a reply?

---

**👤 You:**
> "Send a review request to customer 'John Doe' (ID: cust_987)."

**🤖 AI Agent:**
> Request sent! I have successfully triggered the review invite campaign for John Doe. He will receive an automated request via his preferred channel.


## ❓ FAQ

**Q: How do I get an API Token for GatherUp?**
Log in to GatherUp, navigate to Settings > API, and you will find your Client ID and can generate a Bearer Token.

**Q: What is the difference between Internal Feedback and Online Reviews?**
Internal Feedback (1st-party) is left directly on your GatherUp survey pages. Online Reviews (3rd-party) are retrieved from external sites like Google and Facebook.

**Q: Can I reply to Google or Facebook reviews via the agent?**
Yes! The 'reply_to_online_review' tool allows you to send responses to third-party platforms that support direct API replies, such as Google and Facebook.

**Q: How do I trigger a new review request?**
Use the 'send_review_invite' tool and provide the specific Customer ID. The agent will trigger the automated email or SMS campaign configured for that business.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gatherup](https://vinkius.com/mcp/gatherup)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GatherUp** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gatherup` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GatherUp** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gatherup": {
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
