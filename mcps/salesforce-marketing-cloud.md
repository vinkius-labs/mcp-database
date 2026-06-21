# Salesforce Marketing Cloud MCP Server

Manage campaigns, track member engagement, measure marketing ROI, and optimize lead generation through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/salesforce-marketing-cloud)

## Overview
**Category:** industry-titans
**Tools Count:** 6

## Description
Connect **Salesforce Marketing** to any AI agent.

### What you can do
- **Campaigns** — Search, create, and filter by status
- **Members** — View and add leads/contacts to campaigns
- **Performance** — Aggregate metrics by campaign type

### Who is this for?
- **Marketing Managers** — Campaign health at a glance
- **Demand Gen** — Track lead-to-conversion by campaign
- **Growth Teams** — ROI analysis through conversation


## Available Tools
- **sf_add_campaign_member**: Provide campaignId and either contactId OR leadId (not both). Status defaults to "Sent" but can be set to "Responded", "Registered", etc. based on your campaign member statuses. Returns the created membership record.

Add a lead or contact to a Salesforce marketing campaign for attribution tracking and engagement measurement
- **sf_create_campaign**: Name is required. Type: Email, Conference, Webinar, Trade Show, Public Relations, Advertisement, Banner Ads, Telemarketing. Status defaults to "Planned". Dates use YYYY-MM-DD. budgetedCost is the planned spend. Returns the created campaign with its Salesforce ID.

Create a new marketing campaign in Salesforce with name, type, status, dates, description, and budget
- **sf_campaign_members**: Returns member name, type (Lead or Contact), status (Sent/Responded/etc.), and response date. Use to see who is in a campaign, track engagement, or analyze campaign reach. Essential for campaign ROI and attribution analysis.

Get all leads and contacts enrolled in a specific Salesforce campaign with their membership status and response dates
- **sf_campaign_performance**: Returns the number of campaigns, total leads generated, total conversions, total budgeted cost, and actual cost per campaign type. Provides an instant ROI overview across all marketing channels. Use for marketing dashboard, channel-level performance comparison, or budget allocation analysis.

Get aggregate marketing campaign performance — campaign counts, total leads, conversions, and costs grouped by campaign type
- **sf_campaigns_by_status**: Returns campaigns with lead/contact counts, budget, and conversion data. Use for questions like "which campaigns are currently running?" or "show completed campaigns with their results."

Get Salesforce campaigns filtered by status — Planned, In Progress, Completed, or Aborted — with full metrics
- **sf_search_campaigns**: Returns campaign name, status (Planned/In Progress/Completed/Aborted), type (Email/Conference/Webinar/Advertisement), start/end dates, number of leads generated, contacts converted, budgeted cost, and actual cost. Use when the user asks about marketing initiatives, campaign performance, or budget spend.

Search Salesforce marketing campaigns by name to find initiatives with status, type, budget, and lead/contact conversion metrics


## Installation & Usage

To install and use the **Salesforce Marketing Cloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salesforce-marketing-cloud](https://vinkius.com/mcp/salesforce-marketing-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
