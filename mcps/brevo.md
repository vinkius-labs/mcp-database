# Brevo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brevo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/brevo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/brevo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Automate marketing campaigns via Brevo — send transactional emails, dispatch SMS messages, and manage contacts natively.

## Description
Connect your **Brevo** (formerly Sendinblue) account to any AI agent and execute marketing operations and crucial transactional workflows via natural conversation.

### What you can do

- **Transactional Emails** — Send richly formatted HTML or template-based alerts instantly on demand
- **SMS Dispatch** — Fire immediate SMS campaigns and notifications globally to verified phone numbers
- **Contacts & CRM** — Seamlessly create new user profiles, map attributes, and assign lists structurally

### How it works

1. Enable this MCP integration
2. Provide your Brevo active API Key
3. Execute powerful communication pipelines straight from your chat environment

Skip logging into heavy marketing platforms just to send a manual password reset or subscribe a lead. Instruct the AI and watch emails fly instantly.

### Who is this for?

- **Sales Development** — rapidly create lead contacts adding them to CRM lists automatically after chats
- **Support Teams** — push transactional SMS notifications for ticket resolutions natively while typing
- **IT Administrators** — execute quick service-down or maintenance email blasts directly interacting via prompt
- **Developers** — trigger functional API payload dispatches and test email delivery bypassing Postman


## Available Tools
- **create_crm_contact**: Create a new contact record within the Brevo CRM
- **create_contact_list**: Create a new empty audience list folder for organizing campaigns in Brevo
- **delete_crm_contact**: Permanently delete a CRM contact profile conforming to database compliance
- **get_smtp_account_details**: Retrieve the current Brevo account status, plans, and quota mappings
- **get_contact_attributes**: Retrieve specific profile attributes and metadata for a given contact email
- **list_crm_contacts**: List all contacts stored in the Brevo CRM
- **list_contact_folders**: Retrieve all contact lists and campaign segments structured in the CRM
- **send_transactional_email**: Needs absolute mapped verified domains to avoid DKIM failure bouncing.

Send a transactional email payload via the Brevo SMTP API
- **send_transactional_sms**: 164 phone formats via `/transactionalSMS/sms` successfully bypassing web clients.

Dispatch an automated transactional SMS directly to cellular hardware
- **update_contact_attributes**: Update custom attributes or metadata parameters for a specific CRM contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brevo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a transactional email to test@domain.com saying hello."

**🤖 AI Agent:**
> I've sent the transactional email! The robust Brevo SMTP infrastructure accepted the HTML payload safely. You can track open metrics internally.

---

**👤 You:**
> "Create contact john.doe@mail.com and map their name as John."

**🤖 AI Agent:**
> John's contact record was securely configured inside your CRM architecture! I passed the FIRSTNAME attribute properly over JSON and assigned them neutrally to the general list.

---

**👤 You:**
> "Can you text message 'Server requires reboot' to my admin phone?"

**🤖 AI Agent:**
> The SMS alert has been handed off to the Brevo gateway. It normally delivers under ~200ms depending on explicit telco routes. Logs reflect an affirmative dispatch signal.


## Installation & Usage

To install and use the **Brevo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brevo](https://vinkius.com/mcp/brevo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
