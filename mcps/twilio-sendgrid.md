# Twilio SendGrid MCP Server

Equip your AI agent with capabilities to natively dispatch HTML emails, prune suppression bounce lists, and manage marketing contacts via the SendGrid API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/twilio-sendgrid)

## Overview
**Category:** talk-to-me
**Tools Count:** 16

## Description
Unleash your AI agent over **Twilio SendGrid's** trusted enterprise email platform. Transform your chat interface into a fully-fledged communications command center. By implementing this MCP server, your LLM gains the power to investigate unaddressed hard bounces, dispatch highly contextual custom emails, and automatically organize sprawling marketing directories.

### What you can do

- **Live Email Dispatching** — Dictate a tailored email to your agent and order it to use `dispatch_email` to send fully authenticated outbound HTML campaigns
- **Bounces & Suppression Auditing** — Ask the AI to identify why recent deliveries failed using `list_bounces` and tell it to permanently pardon specific addresses via `delete_bounce`
- **Dynamic Template Inspection** — Fetch all your stored transaction shells (`list_dynamic_templates`) and inspect precise structure iterations to verify UI before broadcasting
- **CRM Growth Automation** — Continuously append or enrich subscriber details straight from conversational prompts by executing `create_marketing_contact` on the fly

### How it works

1. Enable the targeted server component inside your client environment
2. Supply your encrypted `SendGrid API Key` bearing adequate sub-user permissions
3. Engage Cursor or Claude organically to query unsubscriptions or force send notifications immediately

### Who is this for?

- **Customer Success Managers** — organically instruct your AI to search for an angry customer's email across 'bounces', 'spam', or 'unsubscribes' to verify deliverability
- **Software Devs** — test specific edge-cases of dynamic templates bypassing Postman UI just by asking Claude to shoot a trial template straight to your inbox
- **Marketing Integrators** — query the global subscriber list numbers daily alongside other metrics completely through chat


## Available Tools
- **delete_spam_report**: Use with caution — sending to users who report spam can damage your sender reputation.

Remove an email from the spam report suppression list
- **search_contact_by_email**: Returns full contact profile including custom fields, lists, and segments.

Look up a marketing contact by email address
- **get_delivery_stats**: Use YYYY-MM-DD format.

Get global email delivery statistics
- **list_blocked_emails**: Different from bounces — blocks are typically temporary server-level rejections.

List all blocked email addresses
- **create_marketing_contact**: Merges data if the contact already exists.

Creates or updates a marketing contact
- **delete_bounce**: This action is destructive on the suppression record.

Removes an email from the bounce suppression list
- **list_bounces**: Useful for list cleaning.

Lists all bounced email records
- **list_global_unsubscribes**: Lists global unsubscribes
- **list_spam_reports**: Lists user-reported spam complaints
- **get_template_details**: Retrieves details for a specific template
- **list_marketing_contacts**: Lists all marketing contacts
- **list_marketing_lists**: Lists all marketing contact lists
- **list_verified_senders**: Only verified senders can be used in the from_email field.

List all verified sender identities
- **list_single_sends**: List all marketing single-send campaigns
- **list_dynamic_templates**: List all Dynamic Transactional Templates
- **dispatch_email**: Ensure you use a verified sender email in "from_email".

Sends an email via SendGrid SMTP relay


## Installation & Usage

To install and use the **Twilio SendGrid** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/twilio-sendgrid](https://vinkius.com/mcp/twilio-sendgrid)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
