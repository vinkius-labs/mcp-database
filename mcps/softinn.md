# Softinn MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/softinn)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/softinn-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/softinn-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Orchestrate Softinn Hotel PMS — manage reservations, rooms, and guest folios directly from any AI agent.

## Description
Connect your AI agents to **Softinn**, the leading cloud-based Hotel Management System (PMS) and Booking Engine. This MCP provides 10 tools to automate the full lifecycle of your property operations, from real-time availability searches and reservation creation to housekeeping status updates and guest billing management.

### What you can do

- **Reservation Orchestration** — Search for vacant rooms and create guest reservations directly through natural conversation
- **Inventory Control** — List room types and physical rooms to monitor occupancy and technical configurations in real-time
- **Housekeeping Management** — Update room statuses (Clean, Dirty, Maintenance) to keep your operations synchronized
- **Financial Integration** — Access guest folios, monitor outstanding balances, and record payments programmatically
- **Property Insights** — Retrieve hotel metadata and summary configurations for high-level property oversight

### How it works

1. Subscribe to this server
2. Log in to your [**Softinn Merchant Portal**](https://mysoftinn.com/)
3. Contact **support@mysoftinn.com** to request your **API Access Key**
4. Identify your unique **Hotel ID** from your property settings
5. Insert your credentials into the fields below to start managing your hotel operations.

### Who is this for?

- **Hotel Managers** — quickly check room availability and guest details via natural language
- **Reception Staff** — automate the retrieval of daily arrival lists and update room statuses smoothly
- **AEC & PropTech Developers** — integrate hotel PMS data into custom hospitality applications


## Available Tools
- **add_folio_payment**: Record a payment against a guest folio
- **check_availability**: Search for available rooms in the hotel
- **create_reservation**: Create a new guest reservation
- **get_hotel_summary**: Get an overview of the hotel configuration
- **get_reservation_details**: Get details for a specific reservation
- **list_reservation_folios**: Retrieve billing folios for a reservation
- **list_reservations_by_date**: List all reservations for a specific date
- **list_room_types**: List all configured room types for the hotel
- **list_all_rooms**: List all physical rooms and their current metadata
- **update_room_status**: g., Clean, Dirty, Out of Order).

Update the housekeeping or occupancy status of a room


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Softinn** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check room availability in my Softinn hotel from 2024-06-01 to 2024-06-05."

**🤖 AI Agent:**
> Searching Softinn booking engine... I've found 3 available room types for those dates: 1. Deluxe Suite (2 left, RM 350/night), 2. King Room (5 left, RM 280/night), 3. Single Economy (1 left, RM 150/night). Would you like to create a reservation?

---

**👤 You:**
> "Show me the arrival list for today."

**🤖 AI Agent:**
> Retrieving reservations for 2024-04-12... I found 4 arrivals: 1. John Doe (Res: #12345), 2. Jane Smith (Res: #12346), 3. Robert Brown (Res: #12347), 4. Alice White (Res: #12348). All rooms are currently assigned.

---

**👤 You:**
> "Update the status of room 302 to 'Clean'."

**🤖 AI Agent:**
> Connecting to Softinn PMS... I've successfully updated Room 302 (ID: rm_302) to status: 'Clean'. The change is now visible across all property dashboards.


## Installation & Usage

To install and use the **Softinn** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/softinn](https://vinkius.com/mcp/softinn)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
