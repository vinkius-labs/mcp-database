# LEAP Legal MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/leap-legal-1)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/leap-legal-1-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/leap-legal-1-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage legal matters, cards (contacts), and documents via the LEAP API.

## Description
Connect your **LEAP Legal Software** account to any AI agent to streamline your law firm's operations. This MCP server enables your agent to interact with matters, cards (contacts), and legal documentation directly from natural language interfaces.

### What you can do

- **Matter Oversight** — List and retrieve detailed information for legal cases, including status and matter numbers
- **Contact Management** — Manage 'Cards' (people and organizations) and link them to specific legal matters
- **Correspondence Access** — List all documents, emails, and appointments associated with a case
- **Schema Navigation** — Explore legal matter types across different jurisdictions (AU, UK, US, CA, NZ)
- **Record Updates** — Create and update contact cards to ensure your legal database remains accurate

### How it works

1. Subscribe to this server
2. Enter your LEAP API Key, Client ID, and Client Secret
3. Start managing your legal practice from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Solicitors & Lawyers** — Quickly retrieve case details and correspondence history from your development tools
- **Legal Assistants** — Automate the creation of contact cards and monitoring of matter statuses
- **Firm Administrators** — Get instant visibility into the firm's matters and organizational data


## Available Tools
- **list_cards**: List all cards (contacts/organizations)
- **create_new_card**: Requires a JSON body with card details.

Create a new person or organization card
- **get_card_details**: Get details for a specific card (contact)
- **get_matter_details**: Get details for a specific legal matter
- **get_matter_linked_cards**: List all contacts (cards) linked to a matter
- **get_matter_correspondence**: List all correspondence (documents, emails, appointments) for a matter
- **get_matter_documents_only**: List only documents associated with a matter
- **list_legal_matter_types**: ) for a target country code (AU, UK, US, CA, NZ).

List all legal matter types for a country
- **list_matters**: Use this to identify matter IDs for detailed inspection.

List all legal matters (cases)
- **update_existing_card**: Update details for an existing card


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LEAP Legal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active matters in my LEAP account."

**🤖 AI Agent:**
> I've retrieved your matters. You have 15 active cases, including 'Smith vs. Jones (M-101)' and 'Corporate Merger (M-102)'. Which one would you like to explore?

---

**👤 You:**
> "Show correspondence for matter ID 'MAT-12345'."

**🤖 AI Agent:**
> For matter MAT-12345, I found 8 correspondence items: 5 documents (including 'Contract_Draft.pdf'), 2 emails from the client, and 1 upcoming court appointment.

---

**👤 You:**
> "Create a new organization card named 'Legal Tech Solutions'."

**🤖 AI Agent:**
> Successfully created the organization card 'Legal Tech Solutions' in your LEAP database. The new card ID is 'CARD-98765'.


## Installation & Usage

To install and use the **LEAP Legal** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/leap-legal-1](https://vinkius.com/mcp/leap-legal-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
