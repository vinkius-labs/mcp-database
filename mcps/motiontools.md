# MotionTools MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/motiontools)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/motiontools-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/motiontools-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [order-management](../categories/order-management.md)

Manage logistics and delivery operations via MotionTools — track bookings, drivers, and vehicles directly from your AI agent.

## Description
Connect your **MotionTools** account to your AI agent and streamline your urban logistics and fleet management through natural conversation.

### What you can do

- **Booking Management** — List all delivery or hailing bookings and create new ones with pickup and dropoff details.
- **Fleet Oversight** — Access real-time info on your drivers and registered vehicles, including current assignment statuses.
- **Service Area Insights** — List and inspect the geographic zones and boundaries where your operations are active.
- **Customer Records** — View a list of all customers who have booked services in your account.
- **Deep Inspection** — Fetch complete metadata and current status for specific bookings, drivers, or vehicles using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your MotionTools API Token
3. Start managing your logistics from Claude, Cursor, or any MCP client

### Who is this for?

- **Logistics Coordinators** — quickly check the status of a delivery or find an available driver.
- **Fleet Managers** — monitor vehicle assignments and service area coverage directly from your chat.
- **Operations Teams** — automate the creation of new bookings and track their progress in real-time.


## Available Tools
- **create_booking**: Create a new logistics booking
- **get_booking**: Get specific booking details
- **get_driver**: Get specific driver details
- **get_service_area**: Get service area details
- **get_vehicle**: Get specific vehicle info
- **list_bookings**: List logistics bookings
- **list_customers**: List logistics customers
- **list_drivers**: List fleet drivers
- **list_service_areas**: List active service areas
- **list_vehicles**: List fleet vehicles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MotionTools** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my current delivery bookings and their status."

**🤖 AI Agent:**
> I've retrieved your current bookings. You have 3 active deliveries: 'BK-789' (Status: In Progress), 'BK-790' (Status: Scheduled), and 1 other. Would you like the driver details for the one in progress?

---

**👤 You:**
> "Show me the list of active vehicles in the fleet."

**🤖 AI Agent:**
> Fetching fleet vehicles... You have 8 vehicles registered: 6 are currently assigned to drivers ('VAN-01' to 'VAN-06') and 2 are 'available'. Shall I get the metadata for VAN-01?

---

**👤 You:**
> "Create a new booking from 123 Main St to 456 Oak Ave."

**🤖 AI Agent:**
> Initializing new booking... I've successfully created booking 'BK-999' from 123 Main St to 456 Oak Ave. The status is 'unassigned'. Shall I find an available driver in the 'Downtown' service area?


## Installation & Usage

To install and use the **MotionTools** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/motiontools](https://vinkius.com/mcp/motiontools)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
