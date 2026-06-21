# Autenti MCP Server

Sign documents digitally with legal-grade electronic signatures that comply with European eIDAS regulations.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/autenti)

## Overview
**Category:** document-management
**Tools Count:** 12

## Description
Connect your **Autenti** account to any AI agent and take full control of your professional document signing workflows and e-signature compliance through natural conversation.

### What you can do

- **Process Orchestration** — List and manage document signature processes programmatically, retrieving detailed status, high-fidelity metadata, and historical audit data in real-time
- **Dynamic Lifecycle Management** — Discover and execute available actions (Send, Sign, Reject) based on the document's current state to coordinate complex signature workflows
- **Participant Intelligence** — Programmatically add signers and observers to your processes and manage your organizational contact directory to ensure perfectly coordinated collaboration
- **Event Monitoring** — Access and monitor your complete directory of webhooks to receive real-time notifications for incoming document events directly through your agent
- **Operational Visibility** — Access high-fidelity profile metadata for your authenticated user and verify API connectivity directly through your agent for instant reporting

### How it works

1. Subscribe to this server
2. Retrieve your **OAuth Access Token** from the Autenti Developer Portal
3. Start managing your digital trust pipeline from Claude, Cursor, or any MCP client

No more manual status checking of individual contracts or digging through fragmented email threads. Your AI acts as your dedicated digital signature coordinator and compliance architect.

### Who is this for?

- **Legal & Compliance Teams** — instantly retrieve process statuses and execute signature actions using natural language commands
- **Sales Professionals** — automate the dispatch of agreements and monitor signer progress without leaving your creative workspace
- **HR Managers** — orchestrate employment contract workflows and manage participant directories through simple AI queries


## Available Tools
- **check_api_health**: Verify Autenti API connectivity
- **add_new_contact**: Add a contact to your address book
- **create_new_signature_process**: Requires a title and metadata.

Start a new document process
- **execute_process_action**: Use list_available_process_actions first to find valid names.

Execute a discovered action (e.g., Send, Sign, Reject)
- **get_user_account_profile**: Get authenticated user profile
- **get_process_details**: Get details for a specific signature process
- **list_available_process_actions**: Discover possible actions for a process
- **list_saved_contacts**: List your address book contacts
- **list_process_files**: List files within a process
- **list_process_participants**: List signers and observers
- **list_signature_processes**: List all document signature processes
- **list_configured_webhooks**: List active webhooks


## Installation & Usage

To install and use the **Autenti** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/autenti](https://vinkius.com/mcp/autenti)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
