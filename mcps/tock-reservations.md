# Tock Reservations MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tock-reservations)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tock-reservations-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tock-reservations-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to manage restaurant reservations, track guest profiles, and monitor business metrics via the Tock API.

## Description
Integrate **Tock**, the leading reservation and hospitality management platform, directly into your AI workflow. Manage your restaurant or venue reservations and guest directory, track special events and pop-ups, monitor real-time business metrics and occupancy rates, and oversee your hospitality operation using natural language.

### What you can do

- **Reservation Oversight** — List and retrieve detailed information, party sizes, and statuses for all your business reservations.
- **Guest Intelligence** — Monitor guest profiles and history, resolving names, contact details, and total visit counts across your venues.
- **Performance Management** — Access real-time business metrics, resolving total covers, average check size, and occupancy telemetry via chat.
- **Hospitality Auditing** — Retrieve high-level summaries of reservation volume, event activity, and organizational hospitality health instantly.

### How it works

1. Connect the Tock integration to your AI assistant.
2. Authorize using your Tock REST API Key (found in your business dashboard settings).
3. Orchestrate your guest experience and reservation strategy through intuitive conversation.

### Who is this for?

- **Restaurant Managers** — Quickly check daily covers and upcoming reservation counts on the go.
- **Maître d's & Hosts** — Research guest notes and visit history via chat to personalize service.
- **Operations Teams** — Monitor occupancy trends and organizational hospitality metadata instantly.


## Available Tools
- **get_tock_account_metadata**: Retrieve metadata and limits for your Tock account
- **get_business_performance_metrics**: Get a summary of performance metrics for a specific business
- **get_business_detailed_data**: Get detailed settings and information for a specific business
- **quick_hospitality_volume_audit**: Retrieve a high-level summary of reservations, guests, and events
- **get_reservation_details**: Get full content and status for a specific reservation
- **list_managed_businesses**: List all businesses and venues managed in your Tock account
- **list_business_special_events**: List all special events and pop-ups for a specific business
- **list_business_guests**: List all guests registered in the business directory
- **list_business_reservations**: List all reservations for a specific business
- **list_future_scheduled_reservations**: Identify reservations that are scheduled for a future date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tock Reservations** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all reservations for tonight."

**🤖 AI Agent:**
> I've found 15 reservations for tonight, including a party of 4 for 'John Miller' (7:00 PM) and a party of 2 for 'Alice Connor' (8:30 PM). Total expected covers: 45. Would you like to see the guest notes for John Miller?

---

**👤 You:**
> "What are our performance metrics for this week?"

**🤖 AI Agent:**
> This week across your business, you have 350 total covers with an occupancy rate of 85%. The average check size is $75. Performance is up 10% compared to last week. Should I pull the breakdown by day of the week?

---

**👤 You:**
> "Search for guest 'Sarah Connor'."

**🤖 AI Agent:**
> Sarah Connor has visited your venues 5 times. Their last visit was on March 15th at the 'Downtown Bistro'. They are flagged as a 'VIP Guest'. Would you like to see their dietary preferences and special notes?


## Installation & Usage

To install and use the **Tock Reservations** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tock-reservations](https://vinkius.com/mcp/tock-reservations)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
