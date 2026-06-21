# HubSpot Service Hub MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hubspot-service-hub)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hubspot-service-hub-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hubspot-service-hub-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage support tickets, track pipelines, and view customer feedback through natural conversation.

## Description
Connect **HubSpot CRM** to any AI agent — instant access to your full CRM data without switching tabs.

### What you can do
- **Contacts** — Search, create, and manage contacts
- **Companies** — Find companies by name or domain
- **Deals** — Search and create deals with pipeline tracking
- **Tickets** — Create and search support tickets
- **Notes** — Create notes attached to any CRM record
- **Owners** — View all owners and team assignments
- **Pipelines** — List deal and ticket pipeline stages

### Who is this for?
- **Sales Reps** — Manage your CRM without leaving your AI assistant
- **Support Teams** — Create tickets and notes on-the-go
- **RevOps** — Pipeline snapshots and owner assignments
- **Managers** — Full CRM visibility through conversation


## Available Tools
- **hs_create_ticket**: Subject is required. Optionally provide content (detailed description), hs_pipeline (pipeline ID), hs_pipeline_stage (stage ID), and hs_ticket_priority (HIGH, MEDIUM, LOW). If no pipeline is specified, uses the default support pipeline. Returns the created ticket with its HubSpot ID.

Create a new support ticket in HubSpot Service Hub with subject, description, pipeline stage, and priority
- **hs_tickets_by_status**: Returns tickets with subject, priority, and dates. Use when the user asks "how many tickets are open?", "what is waiting for response?", or for support queue analysis. Find stage IDs using hs_ticket_pipelines first.

Get all HubSpot tickets at a specific pipeline stage to analyze queue depth, workload, or resolution bottlenecks
- **hs_list_feedback**: Returns survey name, customer rating/score, survey type (NPS/CSAT/CES), and response content. Use when the user asks about customer satisfaction, NPS scores, or wants to review recent feedback from support interactions.

List customer feedback survey submissions in HubSpot with ratings, survey type, and response content
- **hs_ticket_pipelines**: Returns pipeline name, stage labels, stage IDs (needed for creating/filtering tickets), and display order. Support pipelines define the workflow tickets follow: typically New → Waiting on Contact → Waiting on Us → Closed. Essential for finding stage IDs before ticket operations.

List all ticket/support pipelines in HubSpot with their stages, display order, and internal IDs
- **hs_search_tickets**: Returns ticket subject, current pipeline stage/status, priority (HIGH/MEDIUM/LOW), pipeline name, category, and creation date. Use when the user asks about open tickets, needs to find a specific support case, or wants to check the status of a customer issue.

Search HubSpot Service Hub tickets by subject or keyword to find customer support cases
- **hs_update_ticket**: Only specified fields are updated. Common use: advance hs_pipeline_stage when a case progresses, escalate hs_ticket_priority, or update the subject for clarity. Use when the user says a ticket moved stages, priority changed, or needs correction.

Update an existing HubSpot ticket — change status, priority, subject, or reassign to reflect case progress


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HubSpot Service Hub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for contacts at Acme Corp"

**🤖 AI Agent:**
> 👥 **Contacts at Acme Corp**
| Name | Email | Phone | Lifecycle |
|---|---|---|---|
| John Smith | john@acme.com | +1 555-0123 | Customer |
| Sarah Chen | sarah@acme.com | +1 555-0456 | Lead |

---

**👤 You:**
> "Create a deal: Enterprise Package $50,000"

**🤖 AI Agent:**
> ✅ **Deal Created!**
- Name: Enterprise Package
- Amount: $50,000
- Pipeline: Sales Pipeline
- Stage: Appointment Scheduled

---

**👤 You:**
> "Show me the deal pipeline stages"

**🤖 AI Agent:**
> 📊 **Sales Pipeline**
1. Appointment Scheduled
2. Qualified to Buy
3. Presentation Scheduled
4. Decision Maker Bought-In
5. Contract Sent
6. Closed Won ✅
7. Closed Lost ❌


## Installation & Usage

To install and use the **HubSpot Service Hub** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hubspot-service-hub](https://vinkius.com/mcp/hubspot-service-hub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
