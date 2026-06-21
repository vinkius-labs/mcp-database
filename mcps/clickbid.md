# ClickBid MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clickbid)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/clickbid-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/clickbid-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage auction events, bidders, items, and donations directly via AI.

## Description
The ClickBid integration empowers your AI agent to natively manage your charity auctions and events using natural language.

### What you can do

- **Bidder Management** — Fetch guest lists, register new bidders on the fly, and update their profiles effortlessly.
- **Auction Items** — Manage the event's catalog by retrieving auction items, tracking silent bids, and instantly adding new donated packages.
- **Ticketing & Sales** — Query the complete list of available tickets and identify exactly who has purchased entry to your events.
- **Donations Tracking** — Keep a pulse on fundraising goals by listing and inspecting all monetary donations.

### How it works

1. Retrieve your API Key and API Secret from the ClickBid Admin portal.
2. Add the credentials to this integration.
3. Instruct your AI agent to pull the latest registered bidders or add a new auction item dynamically.

### Who is this for?

- **Event Coordinators** — Look up guest details and bidder IDs instantly during high-traffic events.
- **Nonprofits & Charities** — Track incoming donations and auction items without needing a dashboard.
- **Developers** — Hook custom interfaces or external CRMs to your active ClickBid database.


## Available Tools
- **get_clickbid_item**: Get auction item details
- **list_clickbid_bidders**: List all registered bidders
- **list_clickbid_donations**: List event donations
- **list_clickbid_items**: List auction items
- **list_clickbid_ticket_purchasers**: List ticket purchasers
- **list_clickbid_tickets**: List available tickets
- **create_clickbid_bidder**: Create a new bidder
- **create_clickbid_item**: Create a new auction item
- **get_clickbid_bidder**: Get specific bidder details
- **update_clickbid_bidder**: Update an existing bidder


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ClickBid** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all registered bidders for the upcoming auction."

**🤖 AI Agent:**
> Here is the information you requested based on the execution of the tools.

---

**👤 You:**
> "Retrieve the details for auction item ID 102."

**🤖 AI Agent:**
> Here is the information you requested based on the execution of the tools.

---

**👤 You:**
> "List all ticket purchasers so far."

**🤖 AI Agent:**
> Here is the information you requested based on the execution of the tools.


## Installation & Usage

To install and use the **ClickBid** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clickbid](https://vinkius.com/mcp/clickbid)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
