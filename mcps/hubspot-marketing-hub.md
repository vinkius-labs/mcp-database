# HubSpot Marketing Hub MCP Server

Manage marketing emails, forms, contact lists, campaigns, and landing pages through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/hubspot-marketing-hub)

## Overview
**Category:** industry-titans
**Tools Count:** 6

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
- **hs_form_submissions**: Returns each submission with the field values the visitor entered, submission date, and page URL. Use when the user wants to review lead capture data, check who submitted a form, or analyze form conversion data. You need the form ID — use hs_list_forms to find it.

Get individual form submissions for a specific HubSpot form, showing submitted field values and dates
- **hs_list_campaigns**: Returns campaign name, type, current state, and associated dates. Campaigns group related marketing assets (emails, landing pages, ads) under a single initiative for unified tracking. Use when the user asks about marketing initiatives, campaign performance, or wants to review active campaigns.

List marketing campaigns in HubSpot with name, type, status, and campaign dates
- **hs_list_contact_lists**: Returns list name, type (STATIC for manual lists, DYNAMIC for smart lists with auto-updating criteria), and count of contacts in each list. Use when the user asks about audience segments, marketing lists, wants to know list sizes, or needs to understand audience targeting.

List HubSpot contact lists (static and smart/dynamic) with name, type, and contact count
- **hs_list_forms**: Returns form name, form type (regular/popup/embedded), number of fields, and submission count. Forms are the primary lead capture mechanism in HubSpot. Use when the user asks about lead generation forms, wants to audit form performance, or needs a form ID to check submissions.

List HubSpot forms used for lead capture with name, type, field count, and submission volume
- **hs_list_landing_pages**: Returns page title, publish status (draft/published), URL slug, and full public URL. Landing pages are standalone pages designed for conversion (form fills, downloads). Use when the user asks about landing pages, lead capture pages, or wants to review publishing status.

List HubSpot landing pages with title, publish status, URL slug, and full page URL
- **hs_list_marketing_emails**: Returns email name, subject line, type (regular/automated/blog), current state (draft/published/sent), and publish/send date. Use when the user asks about email campaigns, wants to see recent sends, or needs to check which emails are active.

List marketing emails in HubSpot with name, subject line, send status, type, and publish date


## Installation & Usage

To install and use the **HubSpot Marketing Hub** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hubspot-marketing-hub](https://vinkius.com/mcp/hubspot-marketing-hub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
