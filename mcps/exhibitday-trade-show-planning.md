# ExhibitDay Trade Show Planning MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/exhibitday-trade-show-planning)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/exhibitday-trade-show-planning-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/exhibitday-trade-show-planning-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [event-management](../categories/event-management.md)

Equip your AI agent to manage trade show schedules, track booth shipments, and monitor event budgets via the ExhibitDay API.

## Description
Integrate **ExhibitDay**, the leading trade show planning and exhibition management platform, directly into your AI workflow. Manage your event calendar and booth details, track planning tasks and staff assignments, monitor travel arrangements and material shipments, and oversee your exhibition budgets using natural language.

### What you can do

- **Event Oversight** — List and retrieve detailed planning information, venue details, and booth numbers for all your trade shows.
- **Logistics Intelligence** — Monitor material shipments, travel records, and lodging arrangements across your exhibition projects.
- **Task & Staff Management** — Access and monitor planning tasks and booth staff assignments to ensure operational readiness.
- **Exhibition Auditing** — Retrieve high-level summaries of task completion, budget utilization, and organizational event health instantly.

### How it works

1. Connect the ExhibitDay integration to your AI assistant.
2. Authorize using your ExhibitDay REST API Key (found in your account settings).
3. Orchestrate your trade show logistics and exhibition strategy through intuitive conversation.

### Who is this for?

- **Exhibitor Managers** — Quickly check shipment statuses and staff schedules on the go.
- **Marketing Teams** — Research event budgets and venue details via chat during planning meetings.
- **Operations Teams** — Monitor task completion and organizational exhibition metadata instantly.


## Available Tools
- **get_exhibitday_account_metadata**: Retrieve metadata and limits for your ExhibitDay account
- **get_event_budget_summary**: actual costs.

Get a high-level summary of the budget and expenses for a specific event
- **get_event_detailed_planning_data**: Get detailed settings and logistical information for a specific trade show
- **quick_event_logistics_audit**: Retrieve a high-level summary of tasks, shipments, and travel for an event
- **list_event_booth_staff**: List all team members assigned to staff the booth at a specific event
- **list_trade_show_events**: List all trade shows and exhibitions managed in your ExhibitDay account
- **list_booth_shipments**: List all shipments and freight tracking for booth materials
- **list_planning_tasks**: List all planning and logistical tasks
- **list_event_travel_records**: List all travel and lodging arrangements
- **list_future_scheduled_trade_shows**: Identify trade shows that are scheduled for a future date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ExhibitDay Trade Show Planning** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all trade shows scheduled for this year."

**🤖 AI Agent:**
> I've found 5 trade shows for this year, including 'CES 2024' (Jan), 'NAB Show' (Apr), and 'RSA Conference' (May). Would you like to see the booth details for the NAB Show?

---

**👤 You:**
> "Show me the budget summary for 'TechExpo 2024'."

**🤖 AI Agent:**
> For 'TechExpo 2024', the total estimated budget is $45,000. Actual expenses logged so far are $32,500. Major costs include Booth Space ($15,000) and Sponsorship ($10,000). Should I pull the list of pending tasks?

---

**👤 You:**
> "Check the shipment status for our booth materials."

**🤖 AI Agent:**
> I've retrieved 2 shipments for the upcoming show: 'Main Backdrop' (Delivered via FedEx) and 'Collateral Boxes' (In Transit via UPS, Expected tomorrow). Would you like the tracking link for the UPS shipment?


## Installation & Usage

To install and use the **ExhibitDay Trade Show Planning** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/exhibitday-trade-show-planning](https://vinkius.com/mcp/exhibitday-trade-show-planning)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
