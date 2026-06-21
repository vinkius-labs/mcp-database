# Tactile CRM MCP Server

Connect your AI to Tactile CRM. Query companies, read contact details, and evaluate your sales opportunities and pipelines natively from the terminal.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tactile-crm)

## Overview
**Category:** productivity
**Tools Count:** 9

## Description
Extend the reach of your **Tactile CRM** databases directly into your AI conversational flow utilizing this official Vinkius MCP connector. By granting your LLM localized parsing privileges, you enable it to operate as an intelligent sales assistant that can explore rich business metadata, track sales progression, and summarize unstructured internal notes strictly without relying on graphical CRM interfaces.

### What you can do

- **Client & Corporate Lookups** — Investigate CRM records retrieving specific macro structures invoking `list_companies` and pinpoint specific organizational data operating `get_company_details`.
- **Contact Identification** — Sweep active employee registers querying `list_contacts` and securely extract direct lead data mapping them dynamically with `get_contact_details`.
- **Pipeline Discovery** — Analyze sales cycle projections seamlessly using `list_opportunities` and drill into individual contract values utilizing `get_opportunity_details`.
- **Activity & Note Audits** — Programmatically capture unstructured comments analyzing metadata tracks applying `list_notes` and log engagement events executing `list_activities`.

### How it works

1. Associate the active Tactile CRM integration environment securely over your prompt terminal interface.
2. Accurately assign your corporate `TACTILE_SUBDOMAIN` and specific access matrix (`TACTILE_API_KEY`) obtained from Account Settings > Integrations.
3. Instruct your artificial assistant logically: "Search our CRM companies for 'Acme Corp', evaluate their most recent activities, and retrieve the primary contact email from our pipelines."

### Who is this for?

- **B2B Account Executives** — Instantly review pre-meeting client summaries pulling unformatted notes cleanly into the conversation window bypassing complex web portals.
- **Sales Operation Analysts** — Cross-reference opportunities tracking active funnels programmatically inspecting structural data parameters natively.
- **Customer Success Managers** — Assess real-time organizational footprints logging activities verifying specific company details via simple conversational text evaluations.


## Available Tools
- **list_companies**: Lists all companies (organizations) in the Tactile CRM
- **get_company_details**: Retrieves details for a specific company
- **list_contacts**: Lists all individual contacts (people) in the CRM
- **get_contact_details**: Retrieves details for a specific individual contact
- **list_opportunities**: Lists all sales opportunities (deals) in the pipeline
- **get_opportunity_details**: Retrieves details for a specific sales opportunity
- **list_activities**: Lists recent CRM activities (tasks, calls, emails)
- **list_pipelines**: Lists available sales pipelines
- **list_notes**: Lists general CRM notes


## Installation & Usage

To install and use the **Tactile CRM** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tactile-crm](https://vinkius.com/mcp/tactile-crm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
