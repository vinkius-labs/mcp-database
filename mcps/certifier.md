# Certifier MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/certifier)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/certifier-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/certifier-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Issue branded digital certificates and badges at scale for courses, events, and achievements that recipients can verify online.

## Description
Connect your **Certifier** account to any AI agent and manage your entire digital credentialing workflow through natural conversation.

### What you can do

- **Credential Lifecycle** — Create, update, issue, and send credentials (certificates, badges, diplomas) to recipients.
- **Template Management** — Browse and inspect credential templates to choose the right structure for each certification.
- **Design Control** — List and review visual design templates that define certificate appearance and branding.
- **Recipient Search** — Search across all credentials by recipient name, email, or custom ID to quickly find records.
- **Status Verification** — Confirm API connectivity and check your total credential count.

### How it works

1. Subscribe to this server
2. Enter your Certifier access token (Settings > Developers > Access Tokens)
3. Start issuing credentials from Claude, Cursor, or any MCP client

### Who is this for?

- **Training Coordinators** — issue completion certificates at scale through simple AI commands.
- **HR Teams** — manage employee certifications and track credentialing status.
- **EdTech Platforms** — automate badge and diploma issuance for course completions.


## Available Tools
- **check_certifier_status**: Verify Certifier API connectivity
- **create_credential**: Requires recipient name, email, and template ID.

Create a new credential for a recipient
- **get_credential**: Get full details of a specific credential
- **get_design_template**: Get details of a specific design template
- **get_credential_template**: Get details of a specific credential template
- **issue_credential**: Once issued, it gets a verification URL and cannot revert.

Issue a draft credential to make it official
- **list_credentials**: List all issued credentials
- **list_design_templates**: List all design templates
- **list_credential_templates**: Use template IDs when creating new credentials.

List all credential templates
- **search_credentials**: Search credentials by recipient name or email
- **send_credential**: Send a credential to the recipient via email
- **update_credential**: Only draft credentials can be modified.

Update an existing credential


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Certifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my credential templates in Certifier."

**🤖 AI Agent:**
> I've found 3 templates: 'Course Completion Certificate' (ID: tpl_8a2bc), 'Workshop Badge' (ID: tpl_9d4ef), and 'Professional Diploma' (ID: tpl_1f6gh). Which template would you like to use for a new credential?

---

**👤 You:**
> "Create a certificate for John Smith (john@example.com) using template tpl_8a2bc."

**🤖 AI Agent:**
> Done! Credential created in draft status (ID: cred_xyz789) for John Smith. Would you like me to issue it now and send it to john@example.com?

---

**👤 You:**
> "Search for all credentials issued to anyone at example.com."

**🤖 AI Agent:**
> I found 5 credentials matching 'example.com': 3 issued, 1 draft, and 1 sent. The most recent is a 'Workshop Badge' issued to Sarah Lee yesterday. Would you like to see the full details for any of these?


## Installation & Usage

To install and use the **Certifier** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/certifier](https://vinkius.com/mcp/certifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
