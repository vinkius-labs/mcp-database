# Zoho ZeptoMail MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-zeptomail)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zoho-zeptomail-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zoho-zeptomail-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Send and manage transactional emails with Zoho ZeptoMail and AI agents.

## Description
Connect your **Zoho ZeptoMail** account to any AI agent to automate your transactional email communications and delivery monitoring through natural conversation.

### What you can do

- **Email Automation** — Send single or template-based transactional emails with full HTML and merge variable support.
- **Template Management** — List and utilize pre-defined email templates for consistent branding and messaging.
- **Domain Verification** — Monitor verified domains to ensure high deliverability and sender reputation.
- **Delivery Insights** — Access detailed email logs, delivery reports, and suppression lists to track communication health.

### How it works

1. Subscribe to this server
2. Enter your ZeptoMail Send Mail Token from your Mail Agent settings
3. Select your data center Region (e.g., 'US', 'EU')
4. Start automating your transactional emails from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — automate the sending of service notifications, password resets, and alerts directly from the AI interface.
- **Marketing Operations** — monitor email templates and delivery logs without accessing the ZeptoMail dashboard.
- **Support Teams** — track email delivery status and check suppression lists to resolve customer communication issues quickly.


## Available Tools
- **get_log_details**: Get details for a specific email log
- **list_domains**: List all verified domains
- **list_logs**: List email logs
- **list_suppression_list**: List suppressed email addresses
- **list_templates**: List all email templates
- **send_email**: Requires from_address, to_address, subject, and htmlbody or textbody.

Send a single transactional email
- **send_template_email**: Send an email using a template


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho ZeptoMail** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a password reset email to user 'client@example.com' using the 'Password_Reset_V2' template and include their first name in the merge variables."

**🤖 AI Agent:**
> I successfully sent the password reset email to 'client@example.com' using the 'Password_Reset_V2' template. The merge variables were processed and the email has been queued for delivery.

---

**👤 You:**
> "Check the email logs to see if the welcome email sent to 'newuser@startup.com' yesterday was successfully delivered."

**🤖 AI Agent:**
> I checked the delivery logs. The welcome email sent to 'newuser@startup.com' (Log ID: 94829) was successfully delivered yesterday at 14:32 UTC. The recipient also opened the email.

---

**👤 You:**
> "Verify our active sending domains and check if 'bounced.contact@example.com' is on our suppression list."

**🤖 AI Agent:**
> Your account has 2 verified sending domains ('api-mailer.net' and 'system.app'). I checked the suppression list and 'bounced.contact@example.com' is currently listed due to a hard bounce last week. You won't be able to send emails to this address.


## Installation & Usage

To install and use the **Zoho ZeptoMail** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-zeptomail](https://vinkius.com/mcp/zoho-zeptomail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
