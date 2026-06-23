# Hostfully MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hostfully)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage vacation rental properties, leads, and bookings via Hostfully API.

## Description
Connect your AI agents to Hostfully's Property Management System. This MCP server allows you to list and manage properties, track leads, view guest information, and monitor service providers directly through the Hostfully API. Ideal for automating hospitality operations.


## Available Tools (10)
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


## ❓ FAQ

**Q: Where do I find my Hostfully API Key?**
You can find your API key in the Integration Settings of your Hostfully dashboard.

**Q: Is the Agency UID required?**
It is required for most property and lead related tools. You can find it at the bottom of your Agency Settings page.

**Q: Can I see guest details?**
Yes, the list_guests tool provides access to guest information associated with your agency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hostfully](https://vinkius.com/mcp/hostfully)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hostfully** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hostfully` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hostfully** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hostfully": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
