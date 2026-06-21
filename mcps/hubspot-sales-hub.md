# HubSpot Sales Hub MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hubspot-sales-hub)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hubspot-sales-hub-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hubspot-sales-hub-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage deals, pipelines, products, quotes, and meetings in your HubSpot Sales Hub through natural conversation.

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
- **hs_create_deal**: dealname is required. Specify pipeline and dealstage by their IDs (use hs_list_pipelines to find). Amount is a string representing monetary value. closedate is ISO format. If no pipeline is specified, the deal goes to the default pipeline at its first stage.

Create a new deal/opportunity in the HubSpot sales pipeline with name, stage, amount, and expected close date
- **hs_create_product**: Products serve as catalog items that sales reps can attach to deals as line items or include in quotes. Name is required. Price is the default unit price. SKU (hs_sku) is the internal product identifier. Returns the created product with its HubSpot ID.

Create a new product in the HubSpot product library with name, price, SKU, and description for quoting
- **hs_deals_by_stage**: Returns deals with name, amount, close date, and owner. Use when the user asks "what deals are in Proposal stage?" or "how much revenue is in the Negotiation stage?" or for pipeline stage analysis.

Get all deals at a specific pipeline stage to analyze bottlenecks, forecast revenue, or review stage-specific activity
- **hs_list_meetings**: Returns meeting title, start and end timestamps, outcome/disposition, and associated contacts. Meetings are logged interactions — either via calendar sync or manual entry. Use when the user asks about recent meetings, scheduled calls, or meeting history with a prospect.

List recent meetings logged in HubSpot with title, participants, start/end times, and meeting outcome
- **hs_list_pipelines**: For deals: sales pipeline stages like Appointment Scheduled → Qualified → Proposal → Closed Won. For tickets: support stages like New → Waiting → Closed. Returns pipeline name, stage labels, stage internal IDs (needed for creating/updating deals), and display order. Essential for finding stage IDs before deal operations.

List all deal or ticket pipelines in HubSpot with their stages, display order, and IDs
- **hs_list_quotes**: Returns quote title, approval status (draft/pending/approved/rejected), total amount, expiration date, and associated deal. Quotes are formal price proposals sent to prospects. Use when the user asks about pending quotes, proposal status, or approved pricing documents.

List sales quotes in HubSpot with title, status, total amount, and expiration date
- **hs_search_deals**: Returns deal name, pipeline stage, monetary amount, pipeline name, expected close date, and assigned owner. Use when the user asks about pipeline status, wants to find a specific deal, needs to check deal amounts, or wants to review upcoming closes.

Search HubSpot deals by name to find opportunities in the sales pipeline with stage, amount, and close date
- **hs_search_products**: Returns product name, unit price, SKU, and description. Products are the catalog items that can be added to deals via line items or included in quotes. Use when the user asks about available products, needs to check pricing, or wants to find a product ID for deal line items.

Search HubSpot product library by name to find items available for quoting with prices and SKUs
- **hs_update_deal**: Only specified fields are updated. Common use: advance dealstage when a deal progresses in the pipeline, update amount after negotiation, push closedate when timeline shifts. Use when the user says a deal moved stages, the amount changed, or a close date was updated.

Update an existing HubSpot deal — change stage, amount, close date, or name to reflect pipeline progress


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HubSpot Sales Hub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

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

To install and use the **HubSpot Sales Hub** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hubspot-sales-hub](https://vinkius.com/mcp/hubspot-sales-hub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
