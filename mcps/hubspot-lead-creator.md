# HubSpot Lead Creator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hubspot-lead-creator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hubspot-lead-creator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hubspot-lead-creator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

This MCP does exactly one thing: it extracts customer data from conversations and creates a new Contact in your HubSpot CRM. That's its only function. Incredible for turning your AI into an automated sales assistant.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HubSpot Lead Creator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I just talked to John Doe (john@vinkius.com) and he's interested. Add him as a lead in HubSpot."

**🤖 AI Agent:**
> I have successfully created the contact John Doe in your HubSpot CRM.


## Installation & Usage

To install and use the **HubSpot Lead Creator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hubspot-lead-creator](https://vinkius.com/mcp/hubspot-lead-creator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
