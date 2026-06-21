# Cloutly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloutly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

All-in-one review management platform that helps businesses collect, manage, and respond to reviews from multiple sources.

## Description
Cloutly is an all-in-one review management platform that helps businesses collect, manage, and respond to reviews from multiple sources. It aggregates data from Google, Facebook, Trustpilot, and more into one easy location. Use this MCP server to fetch recent reviews, deploy personalized reputation invitations to customers, and respond programmatically all through a single AI assistant.


## Available Tools
- **list_businesses**: Retrieve all businesses/locations associated with your Cloutly account
- **list_campaigns**: Retrieve active review campaigns for a specific business
- **list_pending_reviews**: Retrieve reviews that have not been replied to yet
- **list_reviews**: Supports filtering by business and pagination.

Retrieve a list of reviews across connected sources
- **reply_to_review**: The reply is posted to the source platform.

Post a reply to a review on its original platform
- **search_reviews_by_author**: Search for reviews from a specific customer by name
- **send_review_invite**: Trigger a review request for a customer via Email or SMS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cloutly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the latest reviews aggregated targeting our main branch in Cloutly."

**🤖 AI Agent:**
> Aggregated 47 reviews across Google, Facebook and Trustpilot. Average rating: 4.6★. Breakdown: 5★ (28), 4★ (12), 3★ (4), 2★ (2), 1★ (1). Sentiment trend: +0.3 over last 30 days.

---

**👤 You:**
> "Send a priority review invitation email to John Doe (john.doe@example.com) for business ID 'xxxx'."

**🤖 AI Agent:**
> Review invitation sent to John Doe (john.doe@example.com) for business 'xxxx'. Priority: high. Delivery method: email. Expected open rate for priority invitations: ~68%.

---

**👤 You:**
> "List all outstanding negative reviews that haven't been replied to in Cloutly."

**🤖 AI Agent:**
> Found 3 negative reviews without replies:
1. Google — 1★ by Mike R. (2 days ago): "Terrible customer service"
2. Facebook — 2★ by Lisa T. (5 days ago): "Long wait times"
3. Trustpilot — 1★ by James K. (1 week ago): "Product arrived damaged"


## ❓ FAQ

**Q: How do I get my Cloutly API key?**
You can generate an API key in your Cloutly dashboard under Developers > Public API to access your permanent key.

**Q: Which review sources are supported?**
Cloutly natively supports Google, Facebook, Trustpilot, TripAdvisor, and many other industry-specific platforms out of the box.

**Q: Can I reply to reviews directly from the MCP?**
Yes, if supported by the channel API, the 'reply_to_review' tool allows you to draft and instantly post responses from your AI.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloutly](https://vinkius.com/mcp/cloutly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cloutly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cloutly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cloutly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cloutly": {
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
