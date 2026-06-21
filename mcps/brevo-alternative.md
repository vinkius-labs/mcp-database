# Brevo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brevo-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/brevo-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/brevo-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Engage customers across email, SMS, and chat with marketing campaigns and transactional messaging that scale with you.

## Description
Connect your **Brevo** account to any AI agent and take full control of your marketing automation and transactional communication workflows through natural conversation.

### What you can do

- **Contact Orchestration** — List and manage your contact database programmatically, retrieving detailed high-fidelity profiles and synchronizing custom attributes in real-time
- **Campaign Intelligence** — Create and monitor high-fidelity email marketing campaigns and retrieve detailed performance reports directly through your agent
- **Transactional Messaging** — Programmatically dispatch single transactional emails via Brevo SMTP to ensure perfectly coordinated customer notifications
- **Audience Discovery** — Access complete directories of contact lists and manage segmentations to maintain high-fidelity targeting for your digital outreach
- **Operational Monitoring** — Access account-level metadata, verified senders, and real-time SMTP delivery statistics for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** (v3) from your Brevo dashboard (SMTP & API settings)
3. Start managing your communication pipeline from Claude, Cursor, or any MCP client

No more manual toggling between campaign tables or digging through SMTP logs. Your AI acts as your dedicated CRM and marketing operations coordinator.

### Who is this for?

- **Digital Marketers** — instantly retrieve campaign engagement metrics and update contact lists using natural language commands
- **Growth Teams** — automate the ingestion of new leads and monitor transactional email health without leaving your workspace
- **Developers** — integrate high-speed email marketing and SMTP features into custom workflows through simple AI queries


## Available Tools
- **get_account**: Get Brevo account details
- **create_email_campaign**: Create an email campaign
- **create_contact**: Create a new contact
- **get_contact**: Get details for a specific contact
- **get_contact_list**: Get details for a specific list
- **get_smtp_statistics**: Get SMTP delivery statistics
- **list_email_campaigns**: List email campaigns
- **list_contacts**: List Brevo contacts
- **list_contact_lists**: List contact lists
- **list_senders**: List approved senders
- **send_email**: Send a transactional email


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brevo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active contacts in my Brevo database."

**🤖 AI Agent:**
> I've retrieved your contact directory. You currently have 150 active subscribers, including @user1 and @user2. Would you like to see the detailed attributes for a specific contact?

---

**👤 You:**
> "Send a transactional email to 'test@example.com' with subject 'Order Confirmed'."

**🤖 AI Agent:**
> Email dispatched! I've successfully sent the 'Order Confirmed' notification to test@example.com via Brevo SMTP. Need help tracking the delivery status?

---

**👤 You:**
> "Show my email campaign engagement statistics."

**🤖 AI Agent:**
> Fetching historical performance... Your last campaign 'Spring Sale' had a 24% open rate and 5% clicks. Total successful deliveries: 4,500. Shall I retrieve the detailed sender metadata for your next run?


## Installation & Usage

To install and use the **Brevo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brevo-alternative](https://vinkius.com/mcp/brevo-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
