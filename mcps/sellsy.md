# Sellsy MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sellsy)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sellsy-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sellsy-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [crm-sales](../categories/crm-sales.md)

Equip your AI agent with full read access to your Sellsy CRM to audit deals, generate invoices overviews, and prospect natively.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sellsy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Identify pending Deals on Sellsy CRM and extract their projected monetary values."

**🤖 AI Agent:**
> I've analyzed your pipeline via `list_deals`. You currently hold 8 active deals labeled 'pending'. Their combined projected valuation totals exactly €24,500. Two key deals lie within the 'Closing/Final Negotiation' phase. Would you like to `get_deal` individually for those two top tier accounts?

---

**👤 You:**
> "Pull the contact information and status for the primary user of 'Company XYZ'."

**🤖 AI Agent:**
> First, I located the enterprise using `search_companies(query: 'Company XYZ')`, matching ID #1059. Then, querying `list_contacts`, I matched the linked employee: Ms. Sarah Jenkin. Her file indicates an active CRM status with the direct tag: 'Account Sponsor'.

---

**👤 You:**
> "Summarize the overarching status of my Sellsy invoices list."

**🤖 AI Agent:**
> I processed `list_invoices`. You possess 32 documented billables in the current view loop. Around 60% are safely flagged as 'PAID'. However, there are 5 critical invoices flagged manually as 'OVERDUE' contributing a gap of near €4,300 to your ledger right now.


## Installation & Usage

To install and use the **Sellsy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sellsy](https://vinkius.com/mcp/sellsy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
