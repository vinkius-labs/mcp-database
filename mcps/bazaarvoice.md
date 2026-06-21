# Bazaarvoice MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bazaarvoice)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bazaarvoice-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bazaarvoice-mcp)
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


## Installation & Usage

To install and use the **Bazaarvoice** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bazaarvoice](https://vinkius.com/mcp/bazaarvoice)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
