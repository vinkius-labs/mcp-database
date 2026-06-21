# Fax.Plus MCP Server

Send and receive faxes digitally through a modern API without physical machines, keeping your business compliant and paperless.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/faxplus)

## Overview
**Category:** communication-messaging
**Tools Count:** 8

## Description
Connect your **Fax.Plus** account to any AI agent and take full control of your digital telephony and fax workflows through natural conversation.

### What you can do

- **Fax Orchestration** — List and monitor all incoming and outgoing faxes and retrieve detailed status updates and delivery metadata programmatically
- **Automated Sending** — Programmatically send new faxes to any international number in E.164 format and add transmission comments directly through your agent
- **Telephony Management** — Search for and list available fax numbers across various countries and area codes to expand your business presence
- **Outbox Oversight** — Track active fax jobs and programmatically cancel pending transmissions before they are completed to save resources
- **Account Visibility** — Retrieve complete profile information, assigned numbers, and team member directories to maintain high-fidelity oversight

### How it works

1. Subscribe to this server
2. Retrieve your **Personal Access Token** from Fax.Plus (Settings > Integrations)
3. Start managing your digital faxing from Claude, Cursor, or any MCP client

No more manual status checking or complex form navigation in the fax dashboard. Your AI acts as your dedicated digital fax and telephony coordinator.

### Who is this for?

- **Operations Managers** — instantly check fax delivery statuses and manage telephony infrastructure using natural language commands
- **Legal & Admin Teams** — automate the sending of critical documents and track receipt without leaving your workspace
- **Business Development** — quickly find and assign new international fax numbers through simple AI queries


## Available Tools
- **get_account_info**: Use this to determine the current identity and account context.

Retrieve current Fax.Plus account details
- **cancel_outbox_job**: Requires the unique outbox job ID.

Cancel a pending fax job
- **get_fax_details**: Includes information about the recipient, sender, and delivery status.

Get details for a specific fax
- **list_faxes**: Use this to monitor communication history and obtain fax IDs.

List received and sent faxes
- **list_fax_numbers**: Includes the number itself and its activation status.

List all assigned fax numbers
- **list_outbox_jobs**: Useful for monitoring ongoing transmissions.

List active or pending fax jobs
- **search_available_numbers**: Useful for expanding telephony infrastructure.

Search for available fax numbers
- **send_fax**: Requires the recipient phone number in E.164 format and allows for optional comments. Files are typically managed via the Fax.Plus outbox logic.

Send a new digital fax


## Installation & Usage

To install and use the **Fax.Plus** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/faxplus](https://vinkius.com/mcp/faxplus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
