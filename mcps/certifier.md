# Certifier MCP Server

Issue branded digital certificates and badges at scale for courses, events, and achievements that recipients can verify online.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/certifier)

## Overview
**Category:** productivity
**Tools Count:** 12

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


## Installation & Usage

To install and use the **Certifier** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/certifier](https://vinkius.com/mcp/certifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
