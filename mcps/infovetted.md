# InfoVetted MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/infovetted)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/infovetted-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/infovetted-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Screen and verify candidate backgrounds with employment checks, education verification, and criminal record searches.

## Description
Connect your **InfoVetted** account to any AI agent and manage background checks through natural conversation.

### What you can do

- **Vetting Requests** — List all vetting requests, create new background checks, check status, and cancel active vettings
- **Screening Contacts** — Manage contacts for screening with full profile data, create new screening contacts, and inspect individual records
- **Package Management** — Browse available vetting packages and their included checks
- **Result Tracking** — Monitor check results with pass/fail status and compliance details
- **Activity History** — View submission and completion timelines

### How it works

1. Subscribe to this server
2. Enter your InfoVetted API Key
3. Start managing background checks from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Teams** — initiate background checks on candidates and track results
- **Compliance Officers** — monitor vetting status and ensure regulatory compliance
- **Staffing Agencies** — manage high-volume screening workflows through AI


## Available Tools
- **cancel_active_vetting**: Cancel a background check
- **check_api_connectivity**: Verify InfoVetted API status
- **create_screening_contact**: Add a new individual for screening
- **create_contact_group**: g., "Engineering Team").

Create a new organization group
- **create_new_vetting_check**: Initiate a background check
- **get_contact_details**: Get details for a specific individual
- **get_vetting_request_status**: Check status of a vetting process
- **list_screening_contacts**: List individuals being screened
- **list_contact_groups**: List organizational contact groups
- **list_vetting_requests**: List all background check requests
- **list_supported_check_types**: ).

List available background check types
- **list_configured_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **InfoVetted** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all active vetting requests and create a new background check for a candidate."

**🤖 AI Agent:**
> Active vetting requests: 8 total. In Progress: 5. Pending: 2. Awaiting Review: 1. Recent: 'Maria Silva' (Standard Package, 60% complete, criminal + employment). 'James Lee' (Premium Package, 40% complete, full background). Contact created: Carlos Mendes (screening_089). Vetting initiated: Standard Background Package (criminal check, employment verification, education verification). Status: Pending. Expected completion: 3-5 business days.

---

**👤 You:**
> "Check the status of Maria Silva's background check and list all screening contacts."

**🤖 AI Agent:**
> Maria Silva (vetting_4521): Status: In Progress (60%). Criminal check: ✅ Clear. Employment verification: ✅ Confirmed (3 employers). Education verification: ⏳ In progress (university confirmation pending). Credit check: ⏳ Pending. Expected completion: Apr 28. Screening contacts: 34 total. Active checks: 8 contacts. Completed: 22. No checks: 4. Would you like to view results or create a new check?

---

**👤 You:**
> "Show completed vetting results and cancel the pending check for candidate #3."

**🤖 AI Agent:**
> Completed vettings (last 30 days): 22 total. ✅ Clear: 18 (82%). ⚠️ Flagged: 3 (14%). ❌ Failed: 1 (4%). Flagged details: 'João Santos' — employment gap (6 months unaccounted). 'Ana Costa' — minor traffic violation. 'David Kim' — degree verification delayed. Cancelled: Pending check for candidate #3 (vetting_4519, 'Lisa Park', Basic Package). Refund: credited. Status: ❌ Cancelled.


## Installation & Usage

To install and use the **InfoVetted** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/infovetted](https://vinkius.com/mcp/infovetted)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
