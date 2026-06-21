# Sharetribe MCP Server

Equip your AI agent to autonomously manage your marketplace. Approve listings, transition transaction states, audit user profiles, and moderate reviews.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sharetribe)

## Overview
**Category:** ecommerce
**Tools Count:** 9

## Description
Grant your AI agent (like Claude or Cursor) absolute administrative dominion over your custom marketplace. The **Sharetribe MCP** equips your LLM to act as a fully autonomous moderator and operations manager. Forget navigating complex vendor panels—now you can manage supply, moderate transactions, and govern your community via natural conversational prompts interacting deeply with your Integration API.

### What you can do

- **Inventory & Listing Moderation** — Crawl through vendor catalogs via `list_listings`. Drill down seamlessly with `get_listing` and publicly publish vetted entries dynamically using `approve_listing`.
- **Live Transaction Steering** — Audit ongoing orders, payments, and booking pipelines with `list_transactions`. Have an order that needs fulfillment? Force operational momentum by applying the `transition_transaction` verb.
- **Community & Vendor Auditing** — Interrogate the platform using `list_users` and `get_user` to investigate behavioral profiles, while constantly scanning aggregated `list_reviews` to maintain healthy interactions.


## Available Tools
- **approve_listing**: Approves a pending listing
- **get_listing**: Retrieves details for a specific listing
- **get_transaction**: Retrieves details for a specific transaction
- **get_user**: Retrieves details for a specific user
- **list_listings**: Lists marketplace listings
- **list_reviews**: Lists marketplace reviews
- **list_transactions**: Lists marketplace transactions
- **list_users**: Lists marketplace users
- **transition_transaction**: g., "confirm", "complete").

Transitions a transaction to a new state


## Installation & Usage

To install and use the **Sharetribe** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sharetribe](https://vinkius.com/mcp/sharetribe)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
