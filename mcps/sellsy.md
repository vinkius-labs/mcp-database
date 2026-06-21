# Sellsy MCP Server

Equip your AI agent with full read access to your Sellsy CRM to audit deals, generate invoices overviews, and prospect natively.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sellsy)

## Overview
**Category:** crm-sales
**Tools Count:** 12

## Description
Connect the **Sellsy CRM** API to your AI workflow to unlock conversational oversight over your entire French-designed commercial hub. By providing exactly Read-Only access, your agent can securely map ongoing deals, review invoice payment statuses, and fetch complete dossiers on existing catalog items and contacts.

### What you can do

- **Client & Prospecting Analysis** — Use natural language to search companies, retrieve full metadata via `company_id`, and pull associated granular contacts directly into the conversational context
- **Sales Pipeline Auditing** — Ask the agent to list all active 'opportunities' and drill down into a specific Deal ID to review its exact stage and monetary potential
- **Billing Integrity** — Prompt your LLM to sweep your current draft, sent, and overdue invoices, including exact estimates given out recently to big leads
- **CRM Activity Surveillance** — Seamlessly extract chronological activity feeds (meetings, calls, tasks) to compile end-of-week reporting automatically

### How it works

1. Simply subscribe to this Sellsy integration server
2. Configure your specific Sellsy V2 API Access token
3. Engage your native terminal IDEs (Cursor/Claude) commanding the AI to cross-reference data

### Who is this for?

- **Sales Managers** — have the AI compile a list of all lagging Deals at 5:00 PM without ever clicking into native reports 
- **B2B Service Account Execs** — instantly invoke `get_contact` combined with `get_company` to read a client history summary right before entering an urgent Zoom call
- **Operation & Finance Teams** — automatically dump your overdue `list_invoices` matrix into a text format so it can be pushed for collection workflows


## Available Tools
- **list_companies**: List all companies (clients, prospects) in the CRM
- **get_company**: Get detailed information about a specific company
- **search_companies**: Search companies by name or keyword
- **list_contacts**: List all contacts in the CRM
- **get_contact**: Get detailed information about a specific contact
- **list_deals**: List all deals (opportunities) in the sales pipeline
- **get_deal**: Get full details of a specific deal (amount, status, pipeline step, company)
- **list_invoices**: List all invoices (draft, sent, paid, overdue)
- **get_invoice**: Get full details of a specific invoice (amount, status, due date)
- **list_estimates**: List all estimates (quotes) sent to prospects
- **list_items**: List all products and services in the catalog
- **list_activities**: List recent CRM activities (calls, emails, meetings, tasks)


## Installation & Usage

To install and use the **Sellsy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sellsy](https://vinkius.com/mcp/sellsy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
