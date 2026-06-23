# Okendo Reviews MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/okendo-reviews)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage customer reviews and social proof via Okendo — track ratings, questions, and product feedback directly from your AI agent.

## Description
Connect your **Okendo** account to your AI agent and gain deep insights into your customer feedback and social proof through natural conversation.

### What you can do

- **Review Monitoring** — List and inspect customer reviews, including star ratings, titles, and body content.
- **Q&A Oversight** — Access customer questions and their respective answers to identify common product concerns.
- **Aggregate Ratings** — Retrieve overall store and product-level star ratings and review counts.
- **Product Intelligence** — View all products tracked in Okendo and access their specific review metrics.
- **Media Access** — List photos and videos uploaded by customers as part of their reviews.
- **Store Settings** — Retrieve high-level configuration and display settings for your Okendo instance.
- **Deep Inspection** — Fetch complete metadata for specific reviews or questions using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your Okendo Subscriber ID (Store ID)
3. Start managing your social proof from Claude, Cursor, or any MCP client

### Who is this for?

- **E-commerce Managers** — quickly check recent reviews or common customer questions without opening the dashboard.
- **Marketing Teams** — identify top-performing products and customer-uploaded media for social campaigns.
- **Customer Support** — monitor product-level feedback and questions to improve service and documentation.


## Available Tools (10)
- **get_aggregate_ratings**: Get store aggregate ratings
- **get_okendo_product_details**: Get product review info
- **get_question_details**: Get specific question details
- **get_review_details**: Get specific review details
- **get_store_settings**: Get Okendo store settings
- **list_question_answers**: List answers for a question
- **list_review_media**: List customer-uploaded media
- **list_okendo_products**: List products tracked in Okendo
- **list_customer_questions**: List customer Q&A questions
- **list_reviews**: List customer reviews


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Okendo Reviews** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the 5 most recent customer reviews."

**🤖 AI Agent:**
> Retrieving recent reviews... I found 5 new ratings: four 5-star reviews and one 4-star review. Customers are highlighting 'Excellent build quality' and 'Fast shipping'. Would you like to read the full body of the 4-star review?

---

**👤 You:**
> "What is the overall star rating for our store?"

**🤖 AI Agent:**
> Fetching aggregate ratings... Your store currently has an overall rating of 4.8 stars based on 1,250 reviews. This is a very strong score! Shall I provide the aggregate ratings for your top 3 products as well?

---

**👤 You:**
> "List the recent questions asked by customers on the site."

**🤖 AI Agent:**
> Retrieving Q&A... I found 3 new questions regarding 'Size and Fit' and 'International Shipping'. 2 of these questions are currently unanswered. Would you like to see the details so you can prepare a response?


## ❓ FAQ

**Q: How do I find my Okendo Subscriber ID?**
You can find your Subscriber ID in the Okendo dashboard settings. It is a unique identifier for your specific store instance.

**Q: Does this support AI-generated review summaries?**
This implementation focuses on retrieving raw review and Q&A data. If your Okendo plan includes AI summaries, they may be accessible within the detailed review metadata.

**Q: Can I see photos uploaded by customers?**
Yes! Use the `list_review_media` tool to retrieve a list of all visual assets (photos and videos) provided by your customers in their feedback.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/okendo-reviews](https://vinkius.com/mcp/okendo-reviews)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Okendo Reviews** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `okendo-reviews` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Okendo Reviews** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "okendo-reviews": {
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
