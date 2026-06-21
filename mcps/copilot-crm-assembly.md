# Copilot CRM (Assembly) MCP Server

Equip your AI agent to manage clients, companies, invoices, and files directly within your Copilot (Assembly) portal.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/copilot-crm-assembly)

## Overview
**Category:** document-management
**Tools Count:** 10

## Description
Integrate **Copilot** (now rebranding to **Assembly**), the leading client portal and CRM platform for service businesses, directly into your AI workflow.

### What you can do

- **Client Management** — List, retrieve, and update client profiles and company associations.
- **Billing Automation** — Monitor invoices, check statuses, and pull payment details via chat.
- **Portal Discovery** — Search for files, messages, and custom fields within your client workspace.

### How it works

1. Connect the Copilot integration to your AI assistant.
2. Authorize using your Copilot API Key (found in Settings > API).
3. Manage your entire client back-office using natural language.

### Who is this for?

- **Agencies & Consultancies** — Streamline client onboarding and project tracking without leaving the chat.
- **Accountants & Law Firms** — Quickly check invoice statuses or pull client documents during planning.
- **Support Teams** — Retrieve client custom fields and portal messages to provide faster assistance.


## Available Tools
- **create_client**: Creates a new client record with identity properties (name, email) and optional company linkages.

Create a new client in the portal
- **get_client_details**: Resolves granular profile data, including contact information, associated company linkages, and system-level metadata.

Get detailed information about a specific client
- **list_clients**: Resolves client identity properties including unique identifiers, names, emails, and account status across the portal system boundary.

List all clients in your Copilot CRM
- **list_companies**: Resolves corporate entity properties such as company IDs, legal names, and primary contact associations.

List all companies in your Copilot CRM
- **list_custom_fields**: Resolves custom field definitions, including field keys, data types, and display labels used across various entities.

Retrieve definitions for custom fields used in CRM
- **list_files**: Resolves file metadata including filenames, storage paths, upload timestamps, and access permissions.

List files uploaded to the Copilot portal
- **list_forms**: Resolves form definitions, including titles, submission endpoints, and configuration metadata.

List intake or feedback forms available
- **list_invoices**: Resolves billing data including amounts, due dates, payment status, and client/company bill-to associations.

List all invoices and their statuses
- **list_portal_messages**: Resolves portal message threads, including sender/receiver identity, message content summary, and timestamps.

List messages sent through the client portal
- **update_client**: Modifies specific attributes like name or account status while preserving other entity properties.

Update existing client details


## Installation & Usage

To install and use the **Copilot CRM (Assembly)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/copilot-crm-assembly](https://vinkius.com/mcp/copilot-crm-assembly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
