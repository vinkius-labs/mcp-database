# Egnyte MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/egnyte)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/egnyte-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/egnyte-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Store and govern enterprise content with intelligent file management, access controls, and compliance monitoring across teams.

## Description
Connect your **Egnyte** enterprise account to any AI agent and take full control of your corporate file sync and share (EFSS) workflows through natural conversation.

### What you can do

- **Content Orchestration** — List and manage files and folders programmatically, including creating new directories and retrieving detailed metadata
- **Secure Sharing** — Programmatically generate shared links with customizable accessibility (public, password, domain) directly from your agent
- **Deep Semantic Search** — Find relevant files and folders across your entire domain using advanced text queries and filters
- **User & Group Visibility** — Retrieve complete directories of users and groups to coordinate permissions and team collaboration
- **Compliance Monitoring** — Access security audit logs and monitor active webhooks to maintain high-fidelity oversight of your corporate data

### How it works

1. Subscribe to this server
2. Register an Internal Application in your Egnyte Developer Portal
3. Retrieve your **Access Token** and **Domain** (e.g., 'acme' from acme.egnyte.com)
4. Start managing your enterprise content from Claude, Cursor, or any MCP client

No more manual folder navigation or complex permission setting in the web UI. Your AI acts as your dedicated IT and content operations coordinator.

### Who is this for?

- **IT Administrators** — instantly retrieve audit logs and manage user groups using natural language commands
- **Operations Leads** — automate folder structures for new projects and monitor shared link usage without leaving your workspace
- **Compliance Officers** — search for sensitive documents and verify access levels through simple AI queries


## Available Tools
- **create_folder**: Create a new folder
- **create_shared_link**: Generate share link
- **delete_item**: Delete file or folder
- **get_account_info**: Get domain info
- **get_audit_logs**: List audit events
- **get_file_metadata**: Get file details
- **list_folder**: List folder contents
- **list_groups**: List user groups
- **list_shared_links**: List all shared links
- **list_users**: List Egnyte users
- **list_webhooks**: List active webhooks
- **search_files**: Search for files


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Egnyte** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all files in the folder '/Shared/Projects/MCP'."

**🤖 AI Agent:**
> I've retrieved the contents of '/Shared/Projects/MCP'. I found 3 files and 2 subfolders, including 'spec_v1.pdf' and 'assets/'. Would you like the metadata for any of these items?

---

**👤 You:**
> "Search for documents containing '2026 marketing budget'."

**🤖 AI Agent:**
> Searching domain... I've found 2 documents: 'Marketing_Budget_v2.xlsx' in /Shared/Finance and 'Q1_Strategy.docx'. Both mention your query. Shall I provide the share links for them?

---

**👤 You:**
> "Show me the last 5 security audit logs."

**🤖 AI Agent:**
> Fetching audit logs... The last 5 events include a password change for user 'John', two folder deletions in /Private, and two successful admin logins. Would you like the detailed timestamps for these?


## Installation & Usage

To install and use the **Egnyte** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/egnyte](https://vinkius.com/mcp/egnyte)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
