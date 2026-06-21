# Judge.me MCP Server

Manage product reviews, questions, and ratings via Judge.me API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/judgeme)

## Overview
**Category:** ecommerce
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Judge.me** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/judgeme](https://vinkius.com/mcp/judgeme)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
