# Mailgun (Transactional Email & Domains) MCP Server

Manage email infrastructure via Mailgun — send transactional emails, monitor domain health, and audit delivery logs.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mailgun-transactional-email-domains)

## Overview
**Category:** ship-it
**Tools Count:** 10

## Description
Connect your **Mailgun** account to any AI agent and take full control of your transactional email delivery, domain health, and suppression management through natural conversation.

### What you can do

- **Transactional Messaging** — Send high-priority transactional or marketing emails directly from your agent, specifying verified domains and custom text bodies securely
- **Domain Health Audit** — Retrieve detailed DNS records and state mappings for your domains, including SPF, DKIM, and MX dependencies to ensure deliverability
- **Suppression Management** — List and audit bounced emails, unsubscribes, and complaints, with the ability to selectively delete suppressions to allow resending
- **Analytics & Statistics** — Query domain-level analytics to track open rates, click-through rates, and general delivery performance in real-time
- **Event Logging** — Extract raw chronological event logs (deliveries, opens, drops, bounces) to investigate delivery failures or anomalous traffic spikes
- **Email Validation** — Use the Mailgun Validation API to check if an email address is deliverable and valid before initiating a send request
- **Template Discovery** — List and retrieve stored HTML Handlebars templates associated with your domains for consistent professional messaging

### How it works

1. Subscribe to this server
2. Enter your Mailgun Private API Key
3. Start managing your email infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Developers** — test transactional email flows and validate domain settings through natural conversation without manual API tools
- **DevOps & SREs** — monitor domain deliverability and investigate delivery logs directly from your workspace for rapid incident response
- **Growth Engineers** — audit campaign stats and manage suppression lists across multiple Mailgun domains efficiently


## Available Tools
- **list_bounces**: Useful to detect out of bounds sending or inactive audiences.

Check bounced email logs and suppression list for a domain
- **delete_bounce**: Irreversible action.

Delete a bounced email from the suppression list
- **get_domain**: Get domain details and DNS records for a Mailgun domain
- **get_stats**: Get analytics and stats for a Mailgun domain
- **get_templates**: List email HTML templates for a Mailgun domain
- **list_domains**: List all configured domains on the Mailgun account
- **list_logs**: List raw event logs (deliveries, opens, drop, bounces) for a domain
- **list_unsubscribes**: List unsubscribed emails for a Mailgun domain
- **send_email**: Send an email using Mailgun
- **validate_email**: Validate an email address via the Mailgun Email Validation API


## Installation & Usage

To install and use the **Mailgun (Transactional Email & Domains)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailgun-transactional-email-domains](https://vinkius.com/mcp/mailgun-transactional-email-domains)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
