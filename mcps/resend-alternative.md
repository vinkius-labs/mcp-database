# Resend MCP Server

Send emails and manage domains via Resend — send transactional emails, track deliveries, manage domains and API keys from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/resend-alternative)

## Overview
**Category:** loved-by-devs
**Tools Count:** 14

## Description
Connect your **Resend** account to any AI agent and take full control of your email infrastructure through natural conversation.

### What you can do

- **Email Sending** — Send transactional emails with HTML/text bodies, attachments, CC/BCC and reply-to addresses
- **Batch Sending** — Send up to 100 emails in a single API call for bulk notifications
- **Email Tracking** — Retrieve sent email details including delivery status, bounces and complaints
- **Domain Management** — Add, verify, update and delete sending domains with DNS record guidance
- **API Key Management** — Create, list and delete API keys with scoped permissions (full_access, sending, domains)
- **Scheduled Emails** — Update or cancel previously scheduled email deliveries

### How it works

1. Subscribe to this server
2. Enter your Resend API Key
3. Start sending emails from Claude, Cursor, or any MCP-compatible client

No more switching to the Resend dashboard to check delivery status or add a new domain. Your AI acts as a dedicated email operations engineer.

### Who is this for?

- **Developers** — quickly send transactional emails, check delivery status and manage domains without leaving your IDE
- **DevOps Engineers** — audit sent email logs, verify domain DNS records and manage API key permissions
- **Product Teams** — send batch notifications, review delivery metrics and manage email templates via conversation


## Available Tools
- **cancel_email**: The email must be in "scheduled" status. Provide the email ID.

Cancel a scheduled email
- **create_api_key**: Requires a name and optionally the permission scope (full_access, sending, domains). Returns the key value which is shown ONLY ONCE — make sure to copy it immediately.

Create a new API key in Resend
- **create_domain**: Requires the domain name (e.g. "example.com"). Optionally set the AWS SES region. Returns the domain ID and the DNS records (SPF, DKIM) you need to configure for verification.

Add a new domain to Resend
- **delete_api_key**: The key will no longer be able to authenticate API requests. Provide the API key ID from list_api_keys. WARNING: this action is irreversible.

Delete an API key from Resend
- **delete_domain**: All DNS records associated with the domain will be invalidated. Provide the domain ID. WARNING: this action is irreversible.

Delete a domain from Resend
- **get_domain**: Provide the domain ID from list_domains.

Get details for a specific domain
- **get_email**: Returns the sender, recipient(s), subject, creation date, last event (delivered, bounced, complained) and scheduled_at if applicable.

Get details for a sent email
- **list_api_keys**: Returns key name, ID, creation date and permission scope (full_access, sending, domains). Note: actual key values are NOT returned for security.

List API keys in your Resend account
- **list_domains**: Each domain shows its name, status (verified, not_verified, pending), region, SPF/DKIM records and creation date. Use this to verify which domains are ready for sending emails.

List verified domains in Resend
- **list_emails**: Returns email ID, from, to, subject, creation date and last event status. Results are paginated and ordered by most recent first.

List recently sent emails
- **send_batch_emails**: Provide a JSON array of email objects, each with from, to, subject and optionally html/text. Each email in the batch is counted individually against your quota. Returns an array of results with IDs for each email.

Send a batch of emails via Resend
- **send_email**: Requires the sender address (from), recipient(s) (to) and subject. Optionally provide HTML body, plain text body, reply-to address, CC/BCC recipients and attachments. The from address must use a verified domain configured in Resend. Returns the email ID for tracking.

Send an email via Resend
- **update_email**: The email must be in "scheduled" status. Provide the email ID and the new scheduled_at timestamp (ISO 8601).

Update a scheduled email
- **verify_domain**: Use this after adding or updating SPF/DKIM records in your DNS provider. Returns the updated domain status.

Verify a domain's DNS records


## Installation & Usage

To install and use the **Resend** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/resend-alternative](https://vinkius.com/mcp/resend-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
