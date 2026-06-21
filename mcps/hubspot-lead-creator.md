# HubSpot Lead Creator MCP Server

This MCP does exactly one thing: it extracts customer data from conversations and creates a new Contact in your HubSpot CRM. That's its only function. Incredible for turning your AI into an automated sales assistant.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/hubspot-lead-creator)

## Overview
**Category:** industry-titans
**Tools Count:** 1

## Description
We refused to build a bloated HubSpot integration that requires terrifying OAuth scopes granting access to your entire sales pipeline, financial data, and deal history. Instead, this MCP server provides a surgical, zero-trust bridge: **just creating a new Contact.**

Your AI agent gains the immediate ability to act as an inbound sales development representative (SDR). During a conversation or when reading an email, if it spots a hot lead, it can instantly dump the name, email, and phone number straight into your HubSpot CRM without human intervention.

### The Superpowers

- **Automated Data Entry:** End manual CRM data entry. The AI parses the context and pushes the lead into HubSpot instantly.
- **Zero-Bloat Integration:** No massive SDKs. It uses a direct `POST` fetch to the HubSpot `/crm/v3/objects/contacts` endpoint. You only need a Private App Access Token.
- **Absolute Containment:** Because this is strictly a "Push-only" creation tool, the agent cannot read your CRM, cannot export your customer list, and cannot delete deals. It only drops leads in. A completely secure, one-way funnel.


## Available Tools
- **create_hubspot_lead**: The "email" field is required. You can also provide firstname, lastname, phone, and company.

Creates a new Contact (Lead) directly in HubSpot CRM


## Installation & Usage

To install and use the **HubSpot Lead Creator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hubspot-lead-creator](https://vinkius.com/mcp/hubspot-lead-creator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
