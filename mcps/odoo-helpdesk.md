# Odoo Helpdesk MCP Server

Create and manage support tickets, track SLAs, organize helpdesk teams — Odoo Helpdesk through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/odoo-helpdesk)

## Overview
**Category:** customer-support
**Tools Count:** 7

## Description
Connect **Odoo ERP** to any AI agent — manage your entire business without switching tabs.

### What you can do
- **CRM** — Search and create leads, track opportunities through your pipeline
- **Contacts** — Find individual contacts and companies, create new partners
- **Sales** — List and manage sales orders with full order details
- **Notes** — Add comments and notes to any record in your Odoo instance

### Who is this for?
- **Sales Teams** — CRM pipeline at your fingertips through AI
- **Account Managers** — Quick access to contact and company information
- **Operations** — Monitor sales orders without switching screens
- **Odoo Administrators** — Query any module through natural conversation


## Available Tools
- **odoo_create_ticket**: ticket record. The name is the ticket subject. Optionally provide the customer email (partner_email), team assignment (team_id from odoo_list_helpdesk_teams), linked customer (partner_id), description, and priority (0=Low, 1=Medium, 2=High, 3=Urgent). The ticket enters the first kanban stage of the assigned team. Use when the user wants to log a support request, report an issue, or create a task for the helpdesk team.

Create a new helpdesk ticket in Odoo for a customer issue with subject, email, team, and priority
- **odoo_list_sla_policies**: sla records showing service level agreements. Returns SLA name, team, target stage, and time targets (days and hours). Use when the user asks about response time commitments, resolution deadlines, or SLA compliance metrics.

List SLA policies configured in Odoo Helpdesk with target response/resolution times per team and stage
- **odoo_list_helpdesk_teams**: team records — the support teams that handle tickets (e.g., "Technical Support", "Billing", "Returns"). Returns team name, member count, and whether SLA tracking is enabled. Use to find team IDs before creating tickets, or when the user asks about the support organization structure.

List all helpdesk teams in Odoo with member count and SLA configuration status
- **odoo_list_ticket_types**: ticket.type records — the classification labels for categorizing tickets. Use when the user asks about available ticket categories or wants to understand how tickets are organized.

List ticket type categories used to classify helpdesk tickets in Odoo (e.g., Bug, Feature Request, Question)
- **odoo_list_tickets**: ticket records ordered by creation date. Returns ticket subject, customer name/email, helpdesk team, kanban stage (e.g., New/In Progress/Solved), priority (0=Low, 1=Medium, 2=High, 3=Urgent), assigned agent, and number of active SLA policies. Optionally filter by team ID. Use when the user asks about support queue, open tickets, team workload, or ticket backlog.

List helpdesk tickets in Odoo with customer, team, kanban stage, priority, assignee, and SLA status
- **odoo_search_tickets**: ticket records by subject/name. Returns matching tickets with customer, team, stage, priority, and assignee. Use when the user wants to find a specific ticket, look up a customer issue, or locate tickets about a particular topic.

Search helpdesk tickets by subject or keyword to find specific customer issues or requests
- **odoo_update_ticket**: ticket record. Use to escalate priority, rename the ticket, reassign to a different agent, or update any writable field. Use when the user wants to modify a ticket that already exists.

Update an existing helpdesk ticket — change subject, priority, assignment, or other properties


## Installation & Usage

To install and use the **Odoo Helpdesk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/odoo-helpdesk](https://vinkius.com/mcp/odoo-helpdesk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
