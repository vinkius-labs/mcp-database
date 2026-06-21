# eSign (e签宝) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/esign-e)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/esign-e-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/esign-e-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Leading digital signature and contract platform in China — manage sign flows, templates, and documents via AI.

## Description
Empower your AI agent to orchestrate your digital agreement lifecycle with **eSign** (e签宝), the premier electronic signature platform in China. By connecting eSign to your agent, you transform complex contract workflows and document signing into a natural conversation. Your agent can instantly list your sign flows, create new signature tasks, manage document templates, and even retrieve signing URLs for participants without you ever needing to navigate the comprehensive eSign portal. Whether you are managing high-volume employee contracts or complex B2B agreements, your agent acts as a real-time legal operations assistant, keeping your documents secure and your business moving.

### What you can do

- **Sign Flow Orchestration** — Create and manage digital signature workflows with full support for documents and signers.
- **Template Management** — Browse predefined document templates to accelerate your contract production.
- **Signature Tracking** — Monitor the real-time status of active sign flows and retrieve execution URLs for participants.
- **Document Control** — Add PDF documents to signature tasks and retrieve download links for completed agreements.
- **Organization Insights** — Retrieve high-level information about your enterprise eSign account and authorization status.

### How it works

1. Subscribe to this server
2. Enter your eSign App ID and App Secret
3. Start managing your digital agreements through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal Operations** — automate contract creation and monitor signing progress through natural language queries.
- **HR Managers** — manage employment contracts and internal policy acknowledgments directly from your AI-powered workspace.
- **Sales Operations** — coordinate B2B agreements and monitor client signatures via a unified AI interface.
- **Enterprise Leaders** — get real-time insights into organization-wide document execution and compliance status.


## Available Tools
- **add_docs**: Add documents to flow
- **add_signers**: Add signers to flow
- **create_sign_flow**: Create a new sign flow
- **download_docs**: Download flow documents
- **get_execute_url**: Get signature URL
- **get_org_info**: Get organization details
- **get_sign_flow**: Get sign flow details
- **list_sign_flows**: List sign flows
- **list_templates**: List sign templates
- **start_flow**: Start sign flow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **eSign (e签宝)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active signature flows on eSign."

**🤖 AI Agent:**
> I've retrieved your active eSign flows. You have 5 tasks in progress, including 'Service Agreement - Client A' and 'New Employee Offer'. Which one would you like to check the status for?

---

**👤 You:**
> "Get the signing URL for account 'acc-8821' in flow 'flow-9920'."

**🤖 AI Agent:**
> I've retrieved the execution URL for the participant. You can send this link to the signer to complete the process: [URL].

---

**👤 You:**
> "Show me all available document templates."

**🤖 AI Agent:**
> I've listed your eSign document templates. You have 3 templates ready for use: 'Standard NDA', 'Employment Contract v2', and 'Sales Agreement'. Would you like to use one of these for a new sign flow?


## Installation & Usage

To install and use the **eSign (e签宝)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/esign-e](https://vinkius.com/mcp/esign-e)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
