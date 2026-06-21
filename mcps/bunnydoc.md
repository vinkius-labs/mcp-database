# BunnyDoc MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bunnydoc)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bunnydoc-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bunnydoc-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Manage eSignatures via BunnyDoc — track document status, manage templates, and coordinate signature requests directly from any AI agent.

## Description
Connect your **BunnyDoc** account to any AI agent and orchestrate your eSignature workflows, document lifecycle, and team collaboration through natural conversation.

### What you can do

- **Signature Requests** — Trigger new document signature requests using pre-defined templates directly from your workspace.
- **Status Oversight** — Monitor the real-time status of envelopes (Draft, Sent, Signed, Completed) using natural language.
- **Template Management** — List all available document templates to ensure consistency in your signing workflows.
- **Team Coordination** — Access your directory of team members and invite new collaborators to the platform.
- **Webhook Automation** — Subscribe to lifecycle events (viewed, signed, completed) to automate your back-office response.
- **Document Auditing** — Retrieve detailed metadata and audit trails for any envelope ID straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your BunnyDoc API Key
3. Start managing your eSignatures from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations & Legal Teams** — quickly check if a contract is signed or send new requests without manual portal work.
- **HR Managers** — monitor onboarding document completion and team access straight from their workflow tools.
- **Developers** — integrate legal signing steps into their environment using natural language.


## Available Tools
- **add_team_member**: Invite a new member to the team
- **create_signature_request**: Create a new signature request from a template
- **get_account_info**: Retrieve core account information
- **get_envelope_status**: Get status of a specific signature request (envelope)
- **get_usage_stats**: Retrieve API usage statistics
- **list_envelopes**: List all signature requests
- **list_team_members**: List all members of the team
- **list_templates**: List all available document templates
- **subscribe_webhook**: Subscribe to signature events via webhook
- **unsubscribe_webhook**: Remove a webhook subscription


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BunnyDoc** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my document templates in BunnyDoc."

**🤖 AI Agent:**
> I've retrieved your templates. You have 3 templates: 'Employment Agreement' (ID: temp_1), 'NDA' (ID: temp_2), and 'Sales Contract' (ID: temp_3).

---

**👤 You:**
> "Show the status of signature request env_99283."

**🤖 AI Agent:**
> The status for request env_99283 ('NDA - John Doe') is 'Completed'. All parties have signed the document as of March 20th.

---

**👤 You:**
> "Send the 'NDA' template to Jane Smith (jane@example.com)."

**🤖 AI Agent:**
> Signature request for the 'NDA' template has been sent to Jane Smith. The new envelope ID is env_12345.


## Installation & Usage

To install and use the **BunnyDoc** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bunnydoc](https://vinkius.com/mcp/bunnydoc)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
