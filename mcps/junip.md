# Junip MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/junip)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/junip-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/junip-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage product reviews, questions, and campaigns via Junip API.

## Description
Empower your AI agents with Junip's scalable product review platform. This MCP server allows you to list and retrieve product reviews, track customer questions and answers, manage display themes, and view review request campaigns directly through the Junip API. Ideal for automating social proof and customer feedback analysis for Shopify stores.


## Available Tools
- **get_account**: Use to verify account identity and access levels.

Retrieves details about your Junip account
- **get_product**: Essential for providing a summary of a product's performance within the store.

Retrieves details for a specific product
- **get_question**: Use this before crafting an official response.

Retrieves details for a specific question
- **get_review**: Returns metadata, custom question responses, and photo/video links (if applicable). Use this when analyzing a specific customer testimonial.

Retrieves details for a specific review
- **list_answers**: Use this to audit response quality and ensure all customer queries are being addressed correctly.

Lists all answers to questions
- **list_campaigns**: Use this to analyze active efforts to collect new customer reviews and feedback.

Lists active review request campaigns
- **list_products**: Includes product names, IDs, and aggregate review metrics. Use this to identify which items have reviews.

Lists all products in your store
- **list_questions**: Returns question text, status, and associated products. Use this to find customer inquiries that require a merchant response.

Lists all customer questions
- **list_reviews**: Returns ratings, review content, and reviewer names. Use this to monitor brand sentiment and identify high-quality social proof.

Lists all product reviews
- **list_themes**: Useful for auditing the visual presentation of reviews on the storefront.

Lists all review display themes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Junip** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all recent product reviews in Junip."

**🤖 AI Agent:**
> I'll fetch the latest reviews from your Junip account.

---

**👤 You:**
> "Show me the questions asked for product ID '123'."

**🤖 AI Agent:**
> I'll retrieve the customer questions associated with that specific product.

---

**👤 You:**
> "Check my active review campaigns."

**🤖 AI Agent:**
> I'll look up the list of configured review request campaigns in Junip.


## Installation & Usage

To install and use the **Junip** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/junip](https://vinkius.com/mcp/junip)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
