# Mailchimp MCP Server

Synchronize marketing contacts — list audiences, control subscriber limits, and edit campaign vectors autonomously.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mailchimp)

## Overview
**Category:** industry-titans
**Tools Count:** 14

## Description
Equip any AI agent with robust Mailchimp marketing capabilities. Integrate your mailing operations transparently to control large audiences, tweak contact statuses dynamically, and trigger organizational insights across your campaigns via conversational prompts.

### What you can do

- **Audience (Lists) Syncing** — Target specific segments, pull overall audience IDs, and grasp performance baselines simply
- **Member Administration** — Unsubscribe, fetch, or permanently store subscriber metadata and profile details without web interfaces
- **Campaign Insights** — Map existing drafted or sent emails across campaigns to keep tabs on global performance metrics programmatically

### How it works

1. Enable the MCP connection under your local profile
2. Input an application-level API token specifically derived from your account
3. Engage directly with LLM shells managing flows through raw texts and pure language operations

### Who is this for?

- **Growth Engineers** — pull massive batches of churned lists instantly for re-validation internally directly avoiding manual filtering
- **Content Marketers** — trace campaign statuses quickly when jumping between different platforms constantly


## Available Tools
- **add_member**: Pass status (subscribed, unsubscribed, cleaned, pending, transactional).

Add a new contact to a Mailchimp audience
- **list_audiences**: List all Mailchimp audiences (lists). Returns audience IDs, names, member counts, and stats
- **list_automations**: List all automation workflows in the account
- **list_campaigns**: Can be used to find a campaign ID.

List Mailchimp campaigns. Returns campaign IDs, types, subjects, send times, and open/click stats
- **create_campaign**: Create a new Mailchimp campaign. Returns campaign ID
- **delete_member**: Requires the list_id and the subscriber MD5 hash (lowercase MD5 of the email).

Archive/remove a subscriber from an audience
- **get_audience**: Only use this when you need detailed statistics or configuration.

Get details of a Mailchimp audience. Returns name, member count, open/click rates, and merge fields configuration
- **get_campaign**: Get full details of a Mailchimp campaign
- **list_members**: Requires an audience ID.

List members (contacts) in a Mailchimp audience. Returns email addresses, status, and tags
- **get_report**: Get Mailchimp campaign performance report
- **search_members**: Search Mailchimp contacts across all audiences by name or email
- **list_segments**: List saved segments for an audience
- **send_campaign**: This action is irreversible. Triggers live email send.

Send a Mailchimp campaign immediately
- **update_member**: Pass json_body with fields like status, merge_fields, tags, etc.

Update subscriber information in an audience


## Installation & Usage

To install and use the **Mailchimp** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailchimp](https://vinkius.com/mcp/mailchimp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
