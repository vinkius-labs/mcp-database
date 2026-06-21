# AwardWallet MCP Server

Manage loyalty points, travel rewards, and itineraries via AwardWallet — monitor your miles and trips directly via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/awardwallet)

## Overview
**Category:** productivity
**Tools Count:** 9

## Description
Connect your **AwardWallet** business account to any AI agent and track your loyalty points, frequent flyer miles, and travel itineraries through natural conversation.

### What you can do

- **Loyalty Tracking** — Monitor balances, expiration dates, and elite status across hundreds of frequent flyer and reward programs
- **Travel Timelines** — Access a unified view of past and upcoming trips, including flights, hotels, and car rentals
- **Itinerary Auditing** — Retrieve detailed metadata and confirmation details for trips shared by your connected users
- **User Access Control** — List and manage users who have authorized your business to access their travel and loyalty data

### How it works

1. Subscribe to this server
2. Enter your AwardWallet Business API Key
3. Start managing your travel rewards from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Business Travelers** — instantly check point balances and trip details without searching through multiple emails
- **Travel Assistants** — coordinate itineraries and monitor expiration dates for team members from a single workspace
- **Operations Teams** — automate the auditing of corporate travel data and loyalty program status for employees


## Available Tools
- **create_auth_url**: Generate an authorization URL for a user to link their AwardWallet account
- **get_account_check**: Verify AwardWallet Business API connection
- **get_account_details**: Get specific details for a loyalty account
- **get_account_history**: Retrieve historical activity for a specific loyalty account
- **get_user_accounts**: Retrieve loyalty account list for a specific user
- **get_user_itineraries**: Retrieve detailed itineraries for a specific user
- **get_user_timeline**: Retrieve the travel timeline for a specific user
- **list_connected_users**: List all AwardWallet users who have authorized your business account
- **list_loyalty_providers**: List all supported loyalty providers


## Installation & Usage

To install and use the **AwardWallet** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/awardwallet](https://vinkius.com/mcp/awardwallet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
