# Dashdoc MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dashdoc)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Equip your AI agent to manage transport orders, fleet, and delivery addresses via the Dashdoc API.

## Description
Integrate **Dashdoc**, the leading transport management system (TMS), directly into your AI workflow. Manage your transport orders, monitor your fleet of trucks and trailers, and track delivery addresses using natural language.

### What you can do

- **Transport Management** — List and retrieve detailed information for all your transport orders and their statuses.
- **Fleet Monitoring** — Track your trucks, trailers, and drivers registered in the Dashdoc system.
- **Address Book** — Manage delivery and pickup addresses and create new records instantly.
- **Partner Insights** — List contacts and business partners associated with your transport operations.

### How it works

1. Connect the Dashdoc integration to your AI assistant.
2. Authorize using your Dashdoc API Key (found in Settings > API).
3. Optimize your logistics and transport operations through intuitive conversation.

### Who is this for?

- **Logistics Managers** — Quickly check transport statuses and fleet availability on the go.
- **Dispatchers** — Access driver information and delivery addresses directly via chat.
- **Supply Chain Teams** — Monitor transport orders and partner contacts during logistics planning.


## Available Tools
- **create_new_address**: Persists site metadata including name, city, and postal code, returning the newly generated system ID for the address.

Add a new address to your Dashdoc address book
- **get_my_user_info**: Returns account-level metadata including user ID, role, and associated fleet/company configuration.

Retrieve metadata for the current authenticated user
- **get_transport_details**: Resolves internal IDs to human-readable names, including full site addresses, contact phone numbers, specific cargo items, and historical status logs.

Get detailed information for a specific transport order
- **list_saved_addresses**: Returns a collection of site objects with GPS coordinates, technical contact details, and site-specific instructions (e.g., gate codes, loading bay requirements).

List all saved delivery and pickup addresses
- **list_transport_contacts**: Resolves business partner identities, including legal names, tax identifiers, and primary communication channels for logistics coordination.

List contacts and business partners
- **list_fleet_drivers**: Returns driver profiles including internal identifiers, professional names, and link to associated vehicle units.

List all drivers registered in the system
- **list_fleet_trailers**: Returns metadata such as trailer type (e.g., refrigerated, tautliner), registration numbers, and fleet assignment status.

List all trailers in your fleet
- **list_transports**: Returns transport metadata including status (e.g., requested, confirmed, ongoing, done), pickup/delivery references, customer IDs, and scheduling timestamps.

List all transport orders in Dashdoc
- **list_fleet_trucks**: Includes license plates, vehicle types, maximum load capacity, and current operational status.

List all trucks in your fleet
- **search_transports_by_reference**: Matches the provided reference keyword against transport-level identifiers and customer references using case-insensitive partial matching.

Search for transport orders by reference keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dashdoc** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all transport orders that are 'Ongoing'."

**🤖 AI Agent:**
> I've found 5 ongoing transports, including 'Order #TR123' from Paris to Lyon and 'Order #TR124' from Berlin to Munich. Would you like to see the assigned drivers for these?

---

**👤 You:**
> "Show me the details for transport order 'TR123'."

**🤖 AI Agent:**
> Transport order 'TR123' is currently 'Loading'. It contains 20 pallets of 'Electronics'. The estimated arrival at destination is tomorrow at 14:00. Should I check the contact info for the pickup point?

---

**👤 You:**
> "List all trucks in our fleet."

**🤖 AI Agent:**
> I've retrieved 12 trucks from your fleet, including 'Truck #01 (AB-123-CD)' and 'Truck #02 (EF-456-GH)'. 8 are currently 'Active' and 4 are 'In Maintenance'. Would you like a list of available trailers?


## ❓ FAQ

**Q: How do I get a Dashdoc API Key?**
Log in to your Dashdoc account, navigate to **Settings > API**, and you can generate or retrieve your API Key there. Ensure your account has API access enabled.

**Q: Can the agent update transport statuses?**
This integration currently focuses on listing and retrieving transport data for analysis. Status updates should be managed via the Dashdoc dashboard or driver mobile app.

**Q: Is fleet data included?**
Yes, you can list your trucks, trailers, and drivers, allowing the agent to provide information on your available transport resources.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dashdoc](https://vinkius.com/mcp/dashdoc)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dashdoc** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dashdoc` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dashdoc** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dashdoc": {
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
