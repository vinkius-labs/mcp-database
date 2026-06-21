# Hudu MCP Server

Document your IT infrastructure with password vaults, knowledge bases, and asset tracking built for managed service providers.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/hudu-alternative)

## Overview
**Category:** developer-tools
**Tools Count:** 12

## Description
Connect your **Hudu** instance to any AI agent and manage your IT documentation through natural conversation.

### What you can do

- **Company Management** — List all client companies, inspect profiles, and create new company records
- **Asset Tracking** — Browse all assets (servers, workstations, network devices), filter by company, inspect details, and create new asset records with tags
- **Password Vault** — List stored passwords filtered by company, and securely retrieve individual password entries with secrets
- **Knowledge Base** — Browse all articles and read full content with metadata for any specific article
- **Procedures & Checklists** — List all procedures filtered by company and inspect detailed steps for operational checklists

### How it works

1. Subscribe to this server
2. Enter your Hudu Instance URL and API Key
3. Start managing IT documentation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **MSPs (Managed Service Providers)** — access client documentation, passwords, and asset inventories without opening the Hudu portal
- **IT Administrators** — track assets, review procedures, and manage knowledge base articles through AI
- **Support Engineers** — quickly retrieve client passwords, asset details, and troubleshooting procedures during incidents


## Available Tools
- **get_article**: Get details for a specific article
- **get_asset**: Get details for a specific asset
- **get_company**: Get details for a specific company
- **get_password**: Get details for a specific password
- **get_procedure**: Get details for a specific procedure
- **list_articles**: List knowledge base articles
- **list_assets**: Can be filtered by company ID.

List assets
- **list_companies**: List all companies in Hudu
- **list_passwords**: Can be filtered by company ID.

List passwords
- **list_procedures**: Can be filtered by company ID.

List procedures
- **create_asset**: Requires asset name and company ID.

Create a new asset
- **create_company**: Requires a name.

Create a new company


## Installation & Usage

To install and use the **Hudu** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hudu-alternative](https://vinkius.com/mcp/hudu-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
