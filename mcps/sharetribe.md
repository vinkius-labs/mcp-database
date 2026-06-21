# Sharetribe MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sharetribe)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sharetribe-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sharetribe-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to autonomously manage your marketplace. Approve listings, transition transaction states, audit user profiles, and moderate reviews.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sharetribe** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve all listings that are currently stuck in the 'pendingApproval' state."

**🤖 AI Agent:**
> Initiating a tactical sweep utilizing `list_listings` aggressively filtered strictly down to the `pendingApproval` state index revealed 4 latent entries idling without resolution. These include "Vintage Bicycle Framework" and three subsequent ambiguous property rental offerings.

---

**👤 You:**
> "Retrieve the details and lifecycle state of the specific transaction bound to the order ID 9c42c2-8491-a9f."

**🤖 AI Agent:**
> Drilling precisely using the `get_transaction` node on string identifier '9c42c2-8491-a9f' unearthed an active, persistent booking element. The current underlying lifecycle state displays officially locked as `transition/preauthorized`.


## Installation & Usage

To install and use the **Sharetribe** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sharetribe](https://vinkius.com/mcp/sharetribe)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
