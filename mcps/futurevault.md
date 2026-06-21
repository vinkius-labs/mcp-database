# FutureVault MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/futurevault)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/futurevault-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/futurevault-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Manage digital vaults, track documents, and oversee folder structures via AI agents with FutureVault.

## Description
Connect your **FutureVault** account to any AI agent to automate your document management and digital vault workflows through the Model Context Protocol (MCP). FutureVault is a secure, high-compliance digital vault platform designed for financial services, wealth management, and high-net-worth individuals. This MCP server enables you to manage your vault directory, retrieve document metadata, and participate in collaborative workflows directly through natural conversation.

### Key Features

- **Vault Orchestration** — List all accessible digital vaults and fetch detailed configuration metadata for each.
- **Directory Structure** — Access and navigate complex folder hierarchies within your vaults to organize sensitive data.
- **Document Oversight** — List documents within specific folders and retrieve complete metadata (owner, tags, status) for individual files.
- **Team & Member Management** — Access vault membership lists and detailed profile information for all users with access.
- **Role Discovery** — List all system roles and permissions to audit your security and access control model.
- **Powerful Search** — Execute global searches across all vaults for specific documents or folders by name or keyword.
- **Real-time Synchronization** — Keep your fiduciary document repository accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your FutureVault API Token (found in your Developer Settings)
3. Start managing your digital vaults from Claude, Cursor, or any MCP client

### Who is this for?

- **Wealth Advisors & Fiduciaries** — quickly check if a client has uploaded a document or verify vault permissions without manual dashboard navigation.
- **Operations Teams** — automate the retrieval of document metadata or audit vault membership via simple AI commands.
- **Financial Planners** — get a real-time overview of folder structures and document statuses for audit readiness.


## Available Tools
- **verify_api_connection**: Check connection
- **get_document_metadata**: Get document details
- **get_folder_details**: Get folder metadata
- **get_member_details**: Get member metadata
- **get_my_identity**: Get current user profile
- **get_vault_details**: Get vault metadata
- **list_folder_documents**: List documents in folder
- **list_vault_folders**: List folders in a vault
- **list_vault_members**: List vault members
- **list_system_roles**: List accessible roles
- **list_digital_vaults**: List all accessible vaults
- **search_vault_content**: Search documents/folders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FutureVault** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all digital vaults I have access to."

**🤖 AI Agent:**
> Retrieving vaults... I found 3 accessible vaults: 'John Smith Personal' (ID: vlt_123), 'Acme Corporate' (ID: vlt_456), and 'Family Trust'.

---

**👤 You:**
> "Search for 'Tax Statement' in all my vaults."

**🤖 AI Agent:**
> Searching content... I found 2 documents matching 'Tax Statement': '2023 Tax Summary.pdf' in the Acme vault and 'Tax Schedule.xlsx' in your personal vault.

---

**👤 You:**
> "Who are the members of the 'Acme Corporate' vault?"

**🤖 AI Agent:**
> Fetching members... The 'Acme Corporate' vault has 4 members: Mike Ross (Admin), Harvey Specter (Member), and 2 others. Would you like their profile details?


## Installation & Usage

To install and use the **FutureVault** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/futurevault](https://vinkius.com/mcp/futurevault)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
