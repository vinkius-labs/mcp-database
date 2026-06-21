# Duo Security (Two-Factor Authentication API) MCP Server

Manage Duo Security users, trigger 2FA authentication, and handle account administration directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/duo-security-two-factor-authentication-api)

## Overview
**Category:** developer-tools
**Tools Count:** 18

## Description
Connect your **Duo Security** instance to your AI agent to streamline identity management and multi-factor authentication workflows.

### What you can do

- **User Lifecycle** — List, create, and modify users. Handle bulk creations and manage the user trash/restoration process.
- **Authentication Control** — Trigger Duo Push, SMS, Phone, or Passcode authentication requests directly from the chat.
- **Pre-authentication Checks** — Determine if a user is authorized to log in and identify available factors before triggering a challenge.
- **Account Administration** — Manage sub-accounts, monitor billing editions, and track telephony credits.
- **Connectivity Testing** — Verify API integration keys and perform liveness checks on the Auth API.

### How it works

1. Subscribe to this server
2. Provide your Duo API Hostname, Integration Key, and Secret Key
3. Start managing security and identity tasks from Claude, Cursor, or any MCP client

### Who is this for?

- **IT Administrators** — quickly audit user lists or update user statuses without navigating the Duo Admin Panel
- **Security Operations (SecOps)** — automate 2FA verification steps or check authentication transaction statuses during investigations
- **DevOps Engineers** — integrate identity checks and account provisioning into automated workflows


## Available Tools
- **auth_status**: Poll for the status of an asynchronous authentication request
- **auth**: Perform second-factor authentication
- **bulk_create_users**: Create up to 100 users in one request
- **check_auth**: Verify integration keys and signature generation
- **create_account**: Create a child account
- **create_user**: Create a new user in Duo
- **delete_account**: Delete a child account
- **get_billing_edition**: Get the billing edition for an account
- **get_telephony_credits**: Get the telephony credits for an account
- **list_accounts**: Retrieve child accounts for Duo MSP partners
- **list_users**: Can filter by username, email, or user_id_list.

Retrieve a paged list of users
- **modify_user**: Change user details
- **ping_auth**: Liveness check for the Auth API
- **preauth**: Determine if a user is authorized to log in and return available factors
- **restore_users**: Restore users from trash
- **set_billing_edition**: Set the billing edition for an account
- **set_telephony_credits**: Set the telephony credits for an account
- **trash_users**: Send users to trash (pending deletion for 7 days)


## Installation & Usage

To install and use the **Duo Security (Two-Factor Authentication API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/duo-security-two-factor-authentication-api](https://vinkius.com/mcp/duo-security-two-factor-authentication-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
