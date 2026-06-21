# Eventbrite MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eventbrite-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eventbrite-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eventbrite-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Eventbrite events — audit organizations, attendees, and orders via AI.

## Description
Empower your AI agent to orchestrate your entire event management ecosystem with **Eventbrite**, the world's largest event technology platform. By connecting Eventbrite to your agent, you transform complex event planning into a natural conversation. Your agent can instantly list your organizations, audit attendee lists, and retrieve order details without you ever touching a dashboard. Whether you are running a small workshop or a massive conference, your agent acts as a real-time event coordinator, ensuring your ticketing and audience data are always accessible and organized.

### What you can do

- **Event Auditing** — List all events in your organization and retrieve detailed metadata, including start times, status, and event URLs.
- **Organization Oversight** — Browse the organizations you belong to and monitor event distribution across your profile.
- **Attendee Management** — Query attendee lists for any event to stay on top of your audience participation and check-ins.
- **Order Auditing** — List all orders for an event to maintain a clear view of your ticketing revenue and sales trends.
- **Resource Intelligence** — List venue details and event categories to ensure your event catalog is correctly organized.

### How it works

1. Subscribe to this server
2. Enter your Eventbrite Private Merchant Token
3. Start managing your events through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Event Organizers** — monitor ticket sales and attendee counts straight from your workflow.
- **Marketing Leads** — verify if new events have been correctly published and categorized for maximum reach.
- **Support Teams** — perform rapid attendee audits and check order details without manual dashboard logins.
- **Operations Leads** — automate event querying to orchestrate cross-functional production teams smoothly.


## Available Tools
- **get_event**: Get details for a specific event
- **get_me**: Get authenticated user info from Eventbrite
- **list_attendees**: List attendees for an event
- **list_categories**: List all Eventbrite categories
- **list_events**: List events for a specific organization
- **list_orders**: List orders for an event
- **list_organizations**: List all organizations the user belongs to
- **list_venues**: List venues for an organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eventbrite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all events for organization ID 12345."

**🤖 AI Agent:**
> I've retrieved your events for that organization. You have 4 active events, including 'AI Workshop' and 'Annual Conference'. Would you like the start times for any of them?

---

**👤 You:**
> "Show me the attendee list for event ID 98765."

**🤖 AI Agent:**
> I've found 15 attendees for this event. Notable participants include 'Marcus R.' and 'Jane Doe'. I can provide the full registration details if you like.

---

**👤 You:**
> "Check recent orders for my upcoming conference."

**🤖 AI Agent:**
> I've scanned your orders. You have 10 new sales today, totaling $450. The most recent order was placed by 'john@doe.com'. Would you like a breakdown by ticket type?


## Installation & Usage

To install and use the **Eventbrite** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eventbrite-alternative](https://vinkius.com/mcp/eventbrite-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
