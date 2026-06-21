# Common Paper MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/common-paper)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/common-paper-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/common-paper-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Common Paper helps you create, send, and sign standard commercial contracts faster. Use this MCP server to automate your contract workflow and track agreement status.

## Description
Connect your **Common Paper** account to any AI agent and manage your commercial contracts through natural conversation.

### What you can do

- **Agreement Management** — List all signed agreements, check the status of pending contracts, and retrieve details for any specific document.
- **Contract Creation** — Send new agreements such as NDAs, Cloud Service Agreements (CSA), and DPAs directly to partners using predefined templates.
- **Workflow Automation** — Streamline your internal processes by programmatically fetching agreement data and triggering contract actions.

### How it works

1. Subscribe to this server
2. Enter your Common Paper API Key
3. Start managing your contracts through Claude, Cursor, or any MCP-compatible client

No more manual drafting or navigating complex legal platforms. Your AI agent becomes your contracting assistant.

### Who is this for?

- **Sales Teams** — quickly send out NDAs or Service Agreements to prospects and track signatures without leaving your workflow.
- **Legal Operations** — audit executed contracts and monitor agreement statuses across the organization.
- **Founders & Executives** — streamline the legal boilerplate required to close deals faster.


## Available Tools
- **create_webhook**: Configure a new webhook to receive contract status updates
- **delete_webhook**: Remove a previously configured webhook
- **get_agreement**: Retrieve detailed information about a specific agreement
- **get_template**: Retrieve details of a specific contract template
- **list_agreements**: Retrieve a list of agreements (contracts) from Common Paper
- **list_signed_agreements**: Quickly list all agreements that have been fully signed
- **list_templates**: Retrieve a list of contract templates available in your account
- **list_webhooks**: Retrieve a list of configured webhooks
- **search_agreements_by_email**: Find agreements associated with a specific recipient email
- **send_agreement**: Create and send a new agreement based on a template


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Common Paper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all signed agreements in Common Paper."

**🤖 AI Agent:**
> I found 5 signed agreements in your Common Paper account. Would you like me to display their details?

---

**👤 You:**
> "Send an NDA agreement to 'partner@example.com' using template ID 'tmpl-xxxx' in Common Paper."

**🤖 AI Agent:**
> I've successfully sent the NDA agreement to 'partner@example.com'. The agreement status is currently pending signature.

---

**👤 You:**
> "Get the current status of agreement 'agr-yyyy' in Common Paper."

**🤖 AI Agent:**
> The agreement 'agr-yyyy' is currently fully executed. It was signed on March 15, 2026.


## Installation & Usage

To install and use the **Common Paper** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/common-paper](https://vinkius.com/mcp/common-paper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
