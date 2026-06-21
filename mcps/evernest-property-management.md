# Evernest Property Management MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/evernest-property-management)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Equip your AI agent to manage rental properties, track tenants, and monitor maintenance via the Evernest API.

## Description
Integrate **Evernest**, the comprehensive digital property management platform, directly into your AI workflow. Manage your rental property portfolio and unit details, track active tenants and lease agreements, monitor maintenance requests and repair statuses, and oversee your property financials using natural language.

### What you can do

- **Property Oversight** — List and retrieve detailed information, occupancy status, and unit configurations for all your managed properties.
- **Tenant Intelligence** — Monitor active tenants and lease terms, resolving contact details and payment history across your portfolio.
- **Maintenance Management** — Access and monitor maintenance tickets and repairs, tracking severity levels and resolution progress.
- **Portfolio Auditing** — Retrieve high-level summaries of property volume, vacancy rates, and organizational portfolio health instantly.

### How it works

1. Connect the Evernest integration to your AI assistant.
2. Authorize using your Evernest API Key (found in your account settings).
3. Orchestrate your property management and real estate investment strategy through intuitive conversation.

### Who is this for?

- **Property Managers** — Quickly check vacancy rates and maintenance status on the go.
- **Real Estate Investors** — Research property financials and tenant history via chat.
- **Maintenance Teams** — Monitor urgent repair tickets and organizational property metadata instantly.


## Available Tools
- **get_evernest_account_metadata**: Retrieve metadata and limits for your Evernest account
- **get_property_detailed_data**: Get detailed settings and financial information for a specific property
- **quick_property_portfolio_audit**: Retrieve a high-level summary of properties, tenants, and maintenance
- **get_tenant_detailed_profile**: Get detailed profile and payment history for a specific tenant
- **list_active_lease_agreements**: List all active lease agreements and contracts
- **list_maintenance_tickets**: List all active and historical maintenance requests
- **list_managed_properties**: List all rental properties managed in your Evernest account
- **list_active_tenants**: List all tenants currently occupying your managed properties
- **list_high_priority_repairs**: Identify maintenance requests that are currently flagged with high severity
- **list_currently_vacant_units**: Identify properties that are currently flagged as vacant


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Evernest Property Management** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all currently vacant properties."

**🤖 AI Agent:**
> I've identified 3 vacant units, including '123 Maple Street' and 'Apartment 4B - Oak Residences'. Would you like to see the listing details for 123 Maple Street?

---

**👤 You:**
> "Show me the maintenance requests flagged as urgent."

**🤖 AI Agent:**
> You have 2 urgent maintenance tickets: 'Leaking Pipe' at 456 Elm Ave and 'Heating System Failure' at 789 Pine St. Both are currently in 'Assigned' status. Should I pull the contractor details for the heating repair?

---

**👤 You:**
> "Get the rent history for tenant 'John Doe'."

**🤖 AI Agent:**
> John Doe (Tenant at 101 Cedar Ln) has a perfect payment history for the last 12 months. Their last payment of $1,500 was received on March 1st. Would you like to see the current lease agreement terms?


## ❓ FAQ

**Q: How do I get an Evernest API Key?**
Log in to your Evernest account, navigate to **Settings > API**, and you can generate or retrieve your unique **API Key** from there. Ensure your account is authorized for API access.

**Q: Does the integration show rent payment status?**
Yes, you can use the get_tenant_detailed_profile tool to retrieve current rent payment history and identify any outstanding balances for specific tenants.

**Q: Can the agent open new maintenance tickets?**
This integration currently focuses on listing and auditing properties, tenants, and maintenance requests. Creating or updating maintenance tickets should be managed via the Evernest dashboard or property manager portal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/evernest-property-management](https://vinkius.com/mcp/evernest-property-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Evernest Property Management** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `evernest-property-management` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Evernest Property Management** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "evernest-property-management": {
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
