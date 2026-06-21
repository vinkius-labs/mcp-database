# Bringg MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bringg)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bringg-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bringg-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Automate final-mile logistics via Bringg — manage delivery tasks, track fleets, and assign drivers directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bringg** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the top 3 most recent active deliveries in the hub."

**🤖 AI Agent:**
> Here are 3 active delivery tasks:
1. (Task ID: 9481...) Delivery to 123 Main St — Status: AT THE PICKUP LOCATION. Driver: John Doe.
2. (Task ID: 7421...) Delivery to 456 Grove St — Status: CREATED. Unassigned.
3. (Task ID: 3109...) Delivery to 789 Pine Ave — Status: ON THE WAY. Driver: Sarah Connor.

Would you like me to manually assign a driver to the second task?

---

**👤 You:**
> "Where is the order for Task ID 3109 and what's its exact timeline?"

**🤖 AI Agent:**
> Pulling timeline for Task 3109… The driver, Sarah Connor, hit 'Start' 15 minutes ago. Current geotracking shows longitude: -74.006, latitude: 40.712. The estimated time of arrival (ETA) is 14:32. Would you like me to add a quick customer note to the order before she arrives?

---

**👤 You:**
> "Force mark task 9481 as complete, the driver forgot to do it."

**🤖 AI Agent:**
> Done. I've sent a mutation to `force_task_complete` for Task 9481. The driver's workflow is manually closed, and the dispatch dashboard should now show this order as successfully finished.


## Installation & Usage

To install and use the **Bringg** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bringg](https://vinkius.com/mcp/bringg)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
