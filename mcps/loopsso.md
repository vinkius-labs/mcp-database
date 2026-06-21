# Loops.so MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/loopsso)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/loopsso-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/loopsso-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage email marketing and transactional emails via Loops.so — handle contacts, campaigns, and events directly from your AI agent.

## Description
Connect your **Loops.so** account to any AI agent to streamline your email marketing and transactional messaging workflows through natural language.

### What you can do

- **Contact Management** — Create, update, find, and delete contacts. Manage mailing list subscriptions and user groups seamlessly.
- **Campaigns & Mailing Lists** — List active campaigns, retrieve specific campaign details, and manage your mailing list infrastructure.
- **Transactional Emails** — Send transactional messages using templates and track their status directly through the agent.
- **Suppression Control** — Check and manage suppression status to ensure your email deliverability remains high.
- **Custom Properties & Events** — Create custom contact properties and trigger events to power your automation workflows.
- **Infrastructure Insights** — List authorized IPs and check API key validity to ensure secure and stable connections.

### How it works

1. Subscribe to this server
2. Enter your Loops API Key
3. Start managing your email audience and campaigns from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing Managers** — quickly update contact segments and check campaign statuses without switching tabs
- **Developers** — trigger transactional emails and test event payloads directly from the code editor
- **Growth Teams** — automate lead ingestion and manage suppression lists through conversational commands


## Available Tools
- **check_api_key**: Check if the Loops API key is valid
- **check_suppression**: Check suppression status for a contact
- **create_campaign**: Create a new campaign (Alpha)
- **create_contact_property**: Create a new contact property
- **create_contact**: Create a new contact in Loops
- **delete_contact**: Delete a contact from Loops
- **find_contact**: Find a contact by email or userId
- **get_campaign**: Get details of a specific campaign (Alpha)
- **get_component**: Get a specific component (Alpha)
- **get_email_message**: Get an email message (Alpha)
- **get_theme**: Get a specific theme (Alpha)
- **list_campaigns**: List all campaigns (Alpha)
- **list_components**: List all components (Alpha)
- **list_contact_properties**: List contact properties
- **list_ips**: List dedicated sending IPs
- **list_mailing_lists**: List all mailing lists
- **list_themes**: List all themes (Alpha)
- **list_transactional_emails**: List transactional emails
- **remove_suppression**: Remove suppression for a contact
- **send_event**: Send an event to Loops
- **send_transactional_email**: Send a transactional email
- **update_campaign**: Update an existing campaign (Alpha)
- **update_contact**: Update an existing contact or create one if it does not exist
- **update_email_message**: Update an email message (Alpha)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Loops.so** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the contact with email 'growth@company.com' and show their details."

**🤖 AI Agent:**
> I've located the contact. Name: Alex Rivera, Status: Subscribed, Source: API. They are currently in the 'Early Adopters' user group.

---

**👤 You:**
> "Send a transactional email to 'user@example.com' using the 'welcome-onboarding' transaction ID."

**🤖 AI Agent:**
> Transactional email sent successfully to user@example.com using the 'welcome-onboarding' template.

---

**👤 You:**
> "List all my active mailing lists and current campaigns."

**🤖 AI Agent:**
> You have 3 mailing lists: 'Main Newsletter', 'Product Updates', and 'Beta Testers'. I also found 2 active campaigns: 'Black Friday 2024' and 'Monthly Digest'.


## Installation & Usage

To install and use the **Loops.so** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/loopsso](https://vinkius.com/mcp/loopsso)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
