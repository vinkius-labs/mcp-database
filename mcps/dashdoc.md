# Dashdoc MCP Server

Equip your AI agent to manage transport orders, fleet, and delivery addresses via the Dashdoc API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dashdoc)

## Overview
**Category:** erp-operations
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Dashdoc** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dashdoc](https://vinkius.com/mcp/dashdoc)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
