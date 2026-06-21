# Listclean MCP Server

Verify and validate email addresses in real-time or batch via the Listclean API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/listclean)

## Overview
**Category:** marketing-automation
**Tools Count:** 5

## Description
Connect your **Listclean** account to any AI agent to automate your email hygiene and deliverability workflows. This MCP server enables your agent to verify single email addresses instantly, process batch validations, and monitor your verification credits directly from natural language interfaces.

### What you can do

- **Real-time Verification** — Instantly check if an email address is clean, dirty, or risky before sending
- **Batch Processing** — Validate large lists of email addresses (up to 3,000 per request) efficiently
- **History Oversight** — Retrieve logs of previously performed single verifications to track your activity
- **Credit Management** — Monitor your remaining verification credits to ensure uninterrupted service
- **Data Quality Audit** — Identify catch-all, disposable, and role-based emails to maintain a high-quality contact list

### How it works

1. Subscribe to this server
2. Enter your Listclean API Key (X-Auth-Token)
3. Start validating your emails from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — Maintain high deliverability by cleaning contact lists via simple natural language commands
- **Sales Teams** — Instantly verify lead emails before reaching out to reduce bounce rates
- **Growth Engineers** — Integrate email validation logic and log monitoring directly into your development tools


## Available Tools
- **verify_batch_emails**: Maximum recommended size is 3,000 per request.

Verify multiple email addresses in one batch
- **check_account_credits**: Check remaining verification credits
- **get_verification_logs**: Retrieve logs of previously verified single emails
- **get_account_profile**: Get account profile details
- **verify_single_email**: Requires a single email string.

Verify a single email address in real-time


## Installation & Usage

To install and use the **Listclean** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/listclean](https://vinkius.com/mcp/listclean)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
