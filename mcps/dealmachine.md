# DealMachine MCP Server

Equip your AI agent to manage real estate leads, track properties, and monitor marketing campaigns via the DealMachine API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dealmachine)

## Overview
**Category:** real-estate
**Tools Count:** 10

## Description
Integrate **DealMachine**, the leading CRM for real estate investors, directly into your AI workflow. Manage your real estate leads, research property ownership and equity data, and monitor direct mail marketing campaigns using natural language.

### What you can do

- **Lead Management** — List, search, and retrieve detailed profiles for your real estate leads.
- **Property Research** — Access full data for tracked properties including owner names, equity, and mortgage information.
- **Campaign Oversight** — Monitor active direct mail and marketing campaigns directly via chat.
- **Team Coordination** — List driving teams and members associated with your account.

### How it works

1. Connect the DealMachine integration to your AI assistant.
2. Authorize using your DealMachine API Key (found in your account settings).
3. Accelerate your real estate investing through intuitive conversation.

### Who is this for?

- **Real Estate Investors** — Quickly check lead details and property equity on the go.
- **Wholesalers** — Research property ownership and manage new leads during field research.
- **Real Estate Teams** — Monitor marketing campaigns and coordinate team activities via chat.


## Available Tools
- **add_new_lead**: Persists a new lead based on property address, initiating property data resolution and owner identification.

Add a new real estate lead to your CRM
- **get_account_details**: Returns account-level metadata including subscription plan, credit balance, and organizational settings.

Retrieve metadata and plan limits for your DealMachine account
- **get_lead_details**: Resolves associated property details, owner contact information, and the history of marketing actions taken.

Get detailed information for a specific real estate lead
- **get_property_details**: Resolves technical data such as estimated equity, mortgage information, deed history, and detailed owner metadata.

Get full data for a specific property including owner and equity
- **list_marketing_campaigns**: Returns campaign summaries including send dates, recipient counts, and engagement metrics.

List all direct mail and marketing campaigns
- **list_real_estate_leads**: Returns lead metadata including property addresses, owner names, and current lead status (e.g., potential, contacted).

List all real estate leads in your DealMachine account
- **list_tracked_properties**: Returns address data and internal property identifiers.

List all properties tracked in the system
- **list_lead_tags**: Returns tag names and identifiers used for filtering leads and properties.

List all tags used to categorize leads and properties
- **list_driving_teams**: Returns a list of teams, active drivers, and their respective roles within the DealMachine workspace.

List all teams and members associated with your account
- **search_leads_by_address**: Matches the search term against property addresses and owner names using partial case-insensitive matching.

Search for leads by address or owner name


## Installation & Usage

To install and use the **DealMachine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dealmachine](https://vinkius.com/mcp/dealmachine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
