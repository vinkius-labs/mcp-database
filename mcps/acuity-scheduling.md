# Acuity Scheduling MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/acuity-scheduling)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/acuity-scheduling-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/acuity-scheduling-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage appointments, availability, calendars, classes, and products for your Acuity Scheduling-powered business through natural conversation.

## Description
Connect your **Acuity Scheduling** (by Squarespace) account to any AI agent and manage your booking operations through natural conversation.

### What you can do

- **Appointments** — List, search, and view booked sessions with client info and intake form answers
- **Availability** — Check real-time available dates and time slots for any service
- **Calendars** — List all providers/instructors and their individual schedules
- **Appointment Types** — Browse all bookable services with pricing and duration
- **Classes** — View group classes with capacity and enrollment
- **Products** — Manage gift certificates and products for sale

### Who is this for?

- **Personal Trainers & Yoga Teachers** — Manage 1-on-1 session bookings effortlessly
- **Wellness Practitioners** — Massage, acupuncture, nutrition consultations
- **Fitness Boutiques** — Small studios using Acuity for scheduling
- **Health Coaches** — Client scheduling with intake forms and availability


## Available Tools
- **check_availability_dates**: Requires Appointment Type ID.

Check which dates have available booking slots for a specific service and month
- **get_account**: Retrieve business profile and account settings from the connected Acuity account
- **get_appointment**: Retrieve the full details of a specific Acuity appointment using its unique ID
- **list_appointment_types**: Shows duration, price, and category.

Retrieve all active bookable service types offered in the Acuity account
- **list_appointments**: Filter by date range.

Retrieve booked appointments from the Acuity Scheduling system, filterable by date range
- **list_available_times**: Essential for booking assistance.

List exactly when someone can book a given Acuity service on a specific date
- **list_calendars**: Retrieve all calendars identifying providers and instructors in Acuity
- **list_classes**: Retrieve group classes scheduled in Acuity, including their capacity and enrolled counts
- **list_products**: Retrieve products or gift certificates available for purchase through Acuity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Acuity Scheduling** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Do I have any open slots for private yoga tomorrow?"

**🤖 AI Agent:**
> Available slots for **Private Yoga Session** tomorrow:

📅 **8:00 AM** — Sarah's calendar ✅
📅 **10:30 AM** — Sarah's calendar ✅
📅 **2:00 PM** — Jake's calendar ✅
📅 **4:30 PM** — Sarah's calendar ✅
📅 **6:00 PM** — Jake's calendar ✅

5 slots available across 2 instructors. The 2:00 PM with Jake is the prime afternoon slot — shall I help you draft a booking confirmation message?


## Installation & Usage

To install and use the **Acuity Scheduling** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/acuity-scheduling](https://vinkius.com/mcp/acuity-scheduling)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
