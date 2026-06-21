# Judge.me MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/judgeme)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/judgeme-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/judgeme-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage product reviews, questions, and ratings via Judge.me API.

## Description
Empower your AI agents with Judge.me's comprehensive product review platform. This MCP server allows you to list and retrieve product reviews, track customer questions and answers, manage coupons, and view shop settings directly through the Judge.me API. Ideal for automating social proof management and customer feedback analysis.


## Available Tools
- **get_product**: Essential for providing a summary of a product's performance.

Retrieves details for a specific product
- **get_question**: Use this before preparing an official answer.

Retrieves details for a specific question
- **get_review**: Returns deep-dive information including metadata and moderation status. Use this when analyzing a particular customer case or response.

Retrieves details for a specific review
- **get_settings**: me app for the shop, including review widgets and email settings. Useful for system configuration auditing.

Retrieves shop settings for Judge.me
- **list_answers**: Use this to audit responses and check if queries have been resolved.

Lists all answers to questions
- **list_coupons**: me (often used as rewards for reviews). Useful for auditing incentive programs.

Lists all active discount coupons
- **list_medias**: Essential for analyzing user-generated content (UGC).

Lists all media (images/videos) attached to reviews
- **list_products**: me. Includes product names, IDs, and aggregate review counts. Use this to identify products for review analysis.

Lists all products in the shop
- **list_questions**: me Q&A feature. Returns question text, status, and IDs. Use this to identify customer inquiries that need answers.

Lists all customer questions
- **list_reviews**: me platform. Returns reviewer names, ratings, review titles, and bodies. Use this to monitor customer sentiment and analyze product feedback.

Lists all product reviews


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Judge.me** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all recent product reviews in Judge.me."

**🤖 AI Agent:**
> I'll fetch the latest reviews from your Judge.me account.

---

**👤 You:**
> "Show me the questions asked for product ID '123'."

**🤖 AI Agent:**
> I'll retrieve the customer questions associated with that specific product.

---

**👤 You:**
> "Check for any active discount coupons."

**🤖 AI Agent:**
> I'll look up the list of active coupons in your Judge.me settings.


## Installation & Usage

To install and use the **Judge.me** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/judgeme](https://vinkius.com/mcp/judgeme)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
