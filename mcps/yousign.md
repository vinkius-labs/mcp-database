# Yousign MCP Server

Manage electronic signatures, signers, and document requests on Yousign — the leading eSignature platform for European teams.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/yousign)

## Overview
**Category:** document-management
**Tools Count:** 8

## Description
Connect your **Yousign** account to any AI agent and manage your electronic signature infrastructure through natural conversation.

### What you can do

- **Signature Lifecycle** — Create new signature requests in draft mode, add signers, and activate requests to send them for signing
- **Request Monitoring** — List and browse all signature processes and retrieve real-time status (draft, ongoing, done, cancelled)
- **Signer Management** — Define and add multiple signers to a request by providing their contact details directly from your agent
- **Document Discovery** — List all files attached to a specific signature request to verify the contents before activation
- **Cancellation Control** — Permanently stop ongoing signature requests and provide custom reasons for termination through simple commands
- **Quota Auditing** — Retrieve API consumption and credit details to monitor your Yousign plan usage and remaining signatures
- **Deep Discovery** — Quickly find unique request, signer, and document IDs required for automated legal workflows

### How it works

1. Subscribe to this server
2. Enter your Yousign API Key
3. Start managing your signing processes through Claude, Cursor, or any MCP-compatible client

No more manual logging into the Yousign dashboard to check if a document was signed. Your AI agent becomes your legal operations assistant.

### Who is this for?

- **Legal & Compliance Teams** — monitor signature statuses and audit document requests through simple chat commands
- **HR Managers** — automate signing processes for employment contracts and verify signer completion via chat
- **Sales Professionals** — track contract signatures and activate new signing requests without manual navigation
- **Operations Managers** — monitor API consumption and manage document lifecycles efficiently


## Available Tools
- **list_requests**: Lists all signature requests in the Yousign organization
- **get_request**: Retrieves details and status for a specific signature request
- **create_request**: Provide a descriptive name for the request.

Creates a new signature request in draft mode
- **add_signer**: Provide the request ID and signer contact details.

Adds a new signer to an existing draft signature request
- **activate_request**: This triggers email notifications to all signers.

Activates a draft signature request and sends it to signers
- **cancel_request**: Provide the request ID and an optional reason for cancellation.

Permanently cancels an ongoing signature request
- **list_documents**: Lists all documents attached to a specific signature request
- **get_consumption**: Retrieves API consumption and quota details


## Installation & Usage

To install and use the **Yousign** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yousign](https://vinkius.com/mcp/yousign)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
