# Bazaarvoice MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bazaarvoice)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Analyze and manage user-generated content via Bazaarvoice — list products, reviews, and customer questions directly from any AI agent.

## Description
Connect your **Bazaarvoice** account to any AI agent and gain deep insights into your customer sentiment and product performance through natural conversation.

### What you can do

- **Product Intelligence** — List and inspect products to understand their market presence and metadata.
- **Review Analysis** — Retrieve and search through customer reviews to identify trends, pain points, and success stories.
- **Q&A Management** — Monitor customer questions and answers to ensure your audience is well-informed and engaged.
- **Category Oversight** — Browse through product categories to understand your catalog structure.
- **Statistical Deep Dives** — Fetch review statistics for specific products to quickly gauge overall customer satisfaction.

### How it works

1. Subscribe to this server
2. Enter your Bazaarvoice API Passkey
3. Start analyzing customer feedback from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — quickly retrieve product ratings and review counts for reporting and strategy.
- **Customer Support Teams** — monitor incoming questions and reviews to provide timely responses.
- **Product Teams** — search reviews for specific keywords to identify feature requests or recurring issues.


## Available Tools
- **get_product**: Get specific product details
- **get_question**: Get specific question details
- **get_review**: Get specific review details
- **get_statistics**: Get review statistics for a product
- **list_answers**: List customer answers
- **list_categories**: List product categories
- **list_products**: List Bazaarvoice products
- **list_questions**: List customer questions
- **list_reviews**: List product reviews
- **search_reviews**: Search reviews by text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bazaarvoice** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all reviews for our best-selling product."

**🤖 AI Agent:**
> I've retrieved the latest reviews. For your top product, I found 25 recent reviews. The average sentiment is highly positive, with common praise for 'durability' and 'design'. Would you like a summary of the most recent 5?

---

**👤 You:**
> "Search for reviews mentioning 'battery life'."

**🤖 AI Agent:**
> Searching through reviews... I found 8 reviews mentioning battery life. 6 are positive, while 2 mention issues after one year of use. Should I summarize the negative ones for the product team?

---

**👤 You:**
> "List current customer questions that need answers."

**🤖 AI Agent:**
> I found 4 unanswered questions. They cover topics like 'compatibility with older models' and 'shipping times to Europe'. Would you like the full text of these questions?


## ❓ FAQ

**Q: Can I search for specific keywords within my product reviews?**
Yes! Use the `search_reviews` tool and provide a text query. Your agent will search through your Bazaarvoice reviews and return those matching your search term.

**Q: How do I get the overall rating statistics for a product?**
Simply use the `get_statistics` action with the target Product ID. It will return a summary of ratings, including average rating and distribution.

**Q: Does this integration allow me to post new answers to customer questions?**
Currently, the toolset is read-only, focusing on retrieving and analyzing content (listing products, reviews, questions). Posting content is not supported in the current version to ensure content moderation workflows are respected.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bazaarvoice](https://vinkius.com/mcp/bazaarvoice)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bazaarvoice** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bazaarvoice` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bazaarvoice** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bazaarvoice": {
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
