# Prosper MCP Server

Manage your Prosper peer-to-peer investments — check account balances, search loan listings, submit bids, and track your portfolio performance.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/prosper)

## Overview
**Category:** finance-accounting
**Tools Count:** 10

## Description
Connect your **Prosper** investment account to any AI agent to automate your peer-to-peer lending strategy. Monitor your portfolio, discover new investment opportunities, and manage your notes through natural conversation.

### What you can do

- **Account Overview** — Retrieve real-time account balances, total value, and available cash for investment via `get_accounts`.
- **Marketplace Discovery** — Search active loan listings using filters like Prosper ratings, biddable status, and credit data with `search_listings`.
- **Automated Bidding** — Submit orders and bids on multiple listings simultaneously to build your portfolio using `submit_order`.
- **Portfolio Tracking** — List and inspect originated loans, specific notes, and payment histories to monitor returns with `list_loans` and `list_notes`.
- **Order Management** — Check the status of submitted orders to confirm successful investments or identify issues using `get_order`.

### How it works

1. Subscribe to this server
2. Enter your Prosper Personal Access Token
3. Start managing your P2P investments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Individual Investors** — automate the search for high-yield listings and track monthly payments without manual logins.
- **Financial Analysts** — pull portfolio data directly into analysis tools to calculate ROI and risk exposure.
- **Developers** — build custom investment bots or dashboards using the Prosper marketplace data.


## Available Tools
- **get_accounts**: Retrieve account balance and investment summaries
- **create_offer**: Generate personalized loan offers for potential borrowers
- **get_loan**: View details of a specific originated loan
- **get_note**: View details of a specific Note investment
- **get_order**: g., BID_SUCCEEDED, INSUFFICIENT_FUNDS).

Check the status of a submitted order
- **list_loans**: View originated loans you have invested in
- **list_notes**: View specific Note investments
- **list_payments**: Retrieve payment history for loans
- **search_listings**: Search for active loan listings to invest in
- **submit_order**: Submit bids on listings


## Installation & Usage

To install and use the **Prosper** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/prosper](https://vinkius.com/mcp/prosper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
