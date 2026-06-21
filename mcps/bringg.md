# Bringg MCP Server

Automate final-mile logistics via Bringg — manage delivery tasks, track fleets, and assign drivers directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/bringg)

## Overview
**Category:** erp-operations
**Tools Count:** 10

## Description
Connect your **Bringg** account to any AI agent and take full control of your final-mile delivery and dispatch operations through natural conversation.

### What you can do

- **Delivery Tasks** — Create, update, list, and cancel delivery tasks dynamically before the truck leaves your hub
- **Fleet Dispatch** — Manually assign specific drivers to tasks, bypassing default optimization algorithms
- **Live Timelines** — Pull real-time geolocated tracking data and status estimates for any active order
- **Force Progression** — Manually trigger task start or completion states to keep the dispatch board accurate
- **Driver CRM** — List all human drivers across the fleet, track their availability, and analyze active limits
- **Customer Database** — Instantly retrieve historical data for past delivery recipients

### How it works

1. Subscribe to this server
2. Enter your Bringg Access Token
3. Start dispatching directly from Claude, Cursor, or any MCP-compatible client

No more jumping between dispatch dashboards. Your AI agent handles the logistics routing.

### Who is this for?

- **Dispatch managers** — reroute drivers, force task states, and check live delivery timelines on the fly
- **Support reps** — instantly check order status and customer history to answer tickets without leaving the CRM
- **Operations teams** — build complex end-of-day delivery analyses and track fleet efficiency
- **Founders & executives** — pull an immediate snapshot of daily active tasks and active fleet resources


## Available Tools
- **assign_driver_to_task**: Manually override optimization and assign a specific driver to a task
- **force_task_complete**: Force a delivery task status to COMPLETE (successfully delivered)
- **create_delivery_task**: Create a new delivery task (order) in the Bringg Delivery Hub
- **cancel_task_dispatch**: Cancel and permanently remove a delivery task from the dispatch schedule
- **get_task_timeline**: Retrieve comprehensive details and live timeline for a specific task
- **list_customer_crm**: List historical delivery recipients (customers) registered in Bringg
- **list_fleet_drivers**: List all human drivers (users) within the Bringg fleet network
- **list_active_tasks**: ` mapping the SaaS dashboard directly isolating pending deliveries.

Retrieve a paginated list of active delivery tasks/orders
- **force_task_start**: Force a delivery task status to START (driver en route)
- **update_task_details**: Modify existing delivery task details such as customer notes or dropoff info


## Installation & Usage

To install and use the **Bringg** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bringg](https://vinkius.com/mcp/bringg)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
