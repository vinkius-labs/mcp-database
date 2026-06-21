# Ziflow MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ziflow)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ziflow-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ziflow-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Enterprise online proofing and content review platform to manage creative workflows with AI.

## Description
Connect your **Ziflow** account to any AI agent to automate your creative review and approval processes through natural conversation.

### What you can do

- **Proof Management** — Search for proofs, track versions, and monitor review statuses across your entire organization.
- **Reviewer Experience** — Generate secure viewer URLs for reviewers and manage contacts/team users efficiently.
- **Decision Tracking** — Submit approval decisions and manage integration properties for cross-platform synchronization.
- **Real-time Events** — Configure and monitor webhooks to stay updated on proofing events in real-time.
- **Asset Organization** — Manage assets associated with product SKUs or project codes directly through the AI interface.

### How it works

1. Subscribe to this server
2. Enter your Ziflow API Token (from Profile settings)
3. Start managing your content reviews from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Creative Agencies** — automate content review cycles and decision tracking for multiple clients.
- **Marketing Departments** — streamline brand approvals and manage internal feedback workflows more efficiently.
- **Production Teams** — track asset versions and generate review links without leaving the project workspace.


## Available Tools
- **create_proof**: Create a new proof
- **create_webhook**: created.

Create a new webhook
- **get_account_info**: Get account profile
- **get_contact_by_email**: Find contact by email
- **get_proof**: Get proof details
- **get_proof_viewer_url**: Generate review link
- **list_folders**: List proof folders
- **list_integration_properties**: List proof metadata
- **list_team_users**: List all users
- **list_webhooks**: List active webhooks
- **search_proofs**: Search for proofs
- **submit_decision**: Submit proof decision


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ziflow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all active proofs in Ziflow."

**🤖 AI Agent:**
> I've retrieved your active proofs. You have 5 proofs in progress, including 'Winter Campaign Video' (v2) and 'Social Media Assets'. Which one would you like to review?

---

**👤 You:**
> "Generate a viewer link for proof ID '12345'."

**🤖 AI Agent:**
> I've generated a secure viewer URL for the proof. Reviewers can access it here: [URL].


## Installation & Usage

To install and use the **Ziflow** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ziflow](https://vinkius.com/mcp/ziflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
