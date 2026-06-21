# Hostfully MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hostfully)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hostfully-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hostfully-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage vacation rental properties, leads, and bookings via Hostfully API.

## Description
Connect your AI agents to Hostfully's Property Management System. This MCP server allows you to list and manage properties, track leads, view guest information, and monitor service providers directly through the Hostfully API. Ideal for automating hospitality operations.


## Available Tools
- **get_agency**: Retrieves details for a specific agency
- **get_lead**: Retrieves details for a specific lead
- **get_property**: Retrieves details for a specific property
- **list_agencies**: Lists all agencies the API key is authorized to access
- **list_guests**: Lists guests associated with an agency
- **list_leads**: Lists leads and bookings for an agency
- **list_owners**: Lists property owners associated with an agency
- **list_properties**: Requires an agencyUid.

Lists all properties belonging to an agency
- **list_service_providers**: Lists service providers (cleaners, maintenance) for an agency
- **list_webhooks**: Lists webhooks configured for an agency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hostfully** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all vacation rental properties in Hostfully."

**🤖 AI Agent:**
> Fetching your property catalog... I found 5 active properties right now. The highlight is 'Sunset Villa (ID: PR-921)' which is currently available for direct bookings, while 'Downtown Loft (ID: PR-304)' remains blocked for maintenance.

---

**👤 You:**
> "Check for new leads in agency UID 'abc-123'."

**🤖 AI Agent:**
> Reviewing agency leads... You have 3 pending inquiries. Lead #409 (Jane Doe) sent an inquiry for the Beach House for next week, and Lead #412 asks about pet policies.

---

**👤 You:**
> "List all service providers for my agency."

**🤖 AI Agent:**
> Here are your service providers: 1. 'Prime Cleaners' (Housekeeping, ID: SP-01). 2. 'QuickFix Plumbing' (Maintenance, ID: SP-02). Let me know if you need to dispatch an emergency order to them.


## Installation & Usage

To install and use the **Hostfully** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hostfully](https://vinkius.com/mcp/hostfully)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
