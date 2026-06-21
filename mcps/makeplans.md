# MakePlans MCP Server

Manage appointments, services, and customers via the MakePlans REST API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/makeplans)

## Overview
**Category:** productivity
**Tools Count:** 8

## Description
Connect your **MakePlans** account to any AI agent to automate your scheduling and appointment management. This MCP server enables your agent to list bookings, find available time slots, manage services and resources, and create customer records directly from natural language interfaces.

### What you can do

- **Appointment Control** — List all scheduled bookings and retrieve detailed metadata and status updates
- **Availability Check** — Query specific services to find available time slots within defined date ranges
- **Resource Oversight** — Manage bookable resources such as staff members, rooms, or specialized equipment
- **Service Catalog** — List all service definitions and appointment types configured in your account
- **Customer CRM** — Create new customer profiles and manage the 'people' database for your business
- **Real-time Scheduling** — Programmatically create new appointments by linking people, services, and time slots

### How it works

1. Subscribe to this server
2. Enter your MakePlans API Key and your Account Name (subdomain)
3. Start managing your calendar from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Service-Based Businesses** — Monitor your appointment calendar and manage availability via simple natural language commands
- **Operations Teams** — Quickly retrieve customer booking histories and update resource assignments without opening the portal
- **Developers** — Integrate scheduling logic and slot availability into your custom internal dashboards


## Available Tools
- **list_appointments**: Use optional params for filtering.

List all bookings/appointments
- **create_new_appointment**: Requires person_id, service_id, and start_at.

Schedule a new booking
- **create_new_customer**: Requires name.

Add a new customer profile
- **get_appointment_details**: Get details for a specific booking
- **list_customers**: List all registered customers
- **list_booking_resources**: List booking resources (staff, rooms, etc.)
- **list_available_services**: List all offered services (appointment types)
- **find_available_slots**: Requires service_id and date parameters.

Find available time slots for a service


## Installation & Usage

To install and use the **MakePlans** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/makeplans](https://vinkius.com/mcp/makeplans)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
