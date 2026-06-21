# SendCloud MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sendcloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sendcloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sendcloud-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Leading email and SMS marketing platform — manage campaigns, templates, and addresses via AI.

## Description
Empower your AI agent to orchestrate your digital communication with **SendCloud**, the premier email and SMS service provider for enterprises. By connecting SendCloud to your agent, you transform complex mailing campaigns, template management, and contact list auditing into a natural conversation. Your agent can instantly send targeted emails, retrieve detailed delivery status, monitor mailing address lists, and even provide performance statistics without you ever needing to navigate the comprehensive SendCloud portal. Whether you are automating transactional notifications or coordinating large-scale marketing newsletters, your agent acts as a real-time communication assistant, keeping your messages accurate and your delivery reliable.

### What you can do

- **Email Orchestration** — Send individual or template-based emails and retrieve real-time delivery status for auditing.
- **Template Management** — Browse and retrieve available email templates to maintain consistent branding across communications.
- **Address List Control** — Create, manage, and monitor mailing address lists and their members directly through the agent.
- **Performance Insights** — Retrieve high-level statistics on email delivery, open rates, and general performance metrics.
- **Account Auditing** — Access general account metadata and monitor your communication usage and limits.

### How it works

1. Subscribe to this server
2. Enter your SendCloud API User and API Key
3. Start managing your digital communication through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Operations** — automate campaign execution and monitor email performance through natural language queries.
- **Customer Success Teams** — coordinate notifications and manage mailing lists directly from your AI-powered workspace.
- **DevOps Engineers** — monitor system communication status and audit account resource usage via a unified AI interface.
- **SendCloud Power Users** — integrate your existing communication workflows into your AI-driven daily routines.


## Available Tools
- **add_address_member**: Add member to address list
- **create_address**: Create address list
- **delete_address**: Delete address list
- **get_email_status**: Get email delivery status
- **get_stats**: Get email statistics
- **get_user_info**: Get account information
- **list_address_members**: List address members
- **list_addresses**: List mailing addresses
- **list_templates**: List email templates
- **send_email**: Send an email


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SendCloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a welcome email to 'mario@example.com' using the 'welcome-template'."

**🤖 AI Agent:**
> I've sent the welcome email to Mario. The message ID is '8821'. You can use this ID to check the delivery status later.

---

**👤 You:**
> "Show me the performance stats for the last month."

**🤖 AI Agent:**
> I've retrieved your SendCloud statistics. Over the last month, you've sent 15,000 emails with a 98% delivery rate and a 25% average open rate. Should I break this down by template?

---

**👤 You:**
> "List all my mailing address lists."

**🤖 AI Agent:**
> I've listed your mailing address lists. You have 3 active lists: 'Newsletter Subscribers', 'VIP Clients', and 'Internal Team'. Which one would you like to see the members for?


## Installation & Usage

To install and use the **SendCloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sendcloud](https://vinkius.com/mcp/sendcloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
