# ClubPlanner MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clubplanner)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/clubplanner-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/clubplanner-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage fitness club memberships, class bookings, and member check-ins with tools designed for health and wellness businesses.

## Description
Connect your **ClubPlanner** fitness management account to any AI agent and simplify how you coordinate your gym, manage member relationships, and track facility usage through natural conversation.

### What you can do

- **Member & Prospect Management** — List active members, track new leads (prospects), and retrieve detailed profile metadata and status.
- **Access Control & Check-ins** — Monitor real-time entry history and record new member check-ins at specific locations.
- **Appointment Scheduling** — List and create appointments for personal training, sales tours, or consultations directly via AI.
- **Contract Oversight** — Query active membership agreements and contracts to monitor renewals and billing cycles.
- **Product Catalog** — Browse available membership types and club products to assist with sales inquiries.
- **Staff Directory** — List registered employees and staff members to coordinate facility operations.
- **Operational Monitoring** — Check your club account metadata and verify API connectivity in real-time.

### How it works

1. Subscribe to this server
2. Enter your ClubPlanner API Key (found in your account settings)
3. Start managing your fitness ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **Gym Owners & Managers** — quickly check daily check-in volume and member statuses via simple AI commands.
- **Front Desk Teams** — record member entries and coordinate training appointments directly from the workspace.
- **Sales & Admin Teams** — monitor prospect pipelines and verify contract availability via the AI assistant.


## Available Tools
- **create_appointment**: Schedule a new appointment
- **create_checkin**: Record a new member check-in
- **create_prospect**: Add a new prospect to ClubPlanner
- **get_me**: Get club account information
- **get_member**: Get details for a specific member
- **list_appointments**: List scheduled appointments
- **list_checkins**: List recent member check-ins
- **list_contracts**: List active membership contracts
- **list_members**: List all club members
- **list_products**: List available products/memberships
- **list_prospects**: List potential members (prospects) in ClubPlanner
- **list_staff**: List club staff members


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ClubPlanner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active members in my ClubPlanner account."

**🤖 AI Agent:**
> I've retrieved the member directory. You have 150 active members including 'John Doe', 'Sarah Miller', and 'Mike Ross'. Which one would you like to see the profile or check-in history for?

---

**👤 You:**
> "Record a check-in for member 'mem_10293' at the main facility."

**🤖 AI Agent:**
> Check-in recorded! I've logged the entry for member mem_10293 at your main facility. Their membership status was verified as 'Active'.

---

**👤 You:**
> "Show me the appointments scheduled for tomorrow."

**🤖 AI Agent:**
> Fetching schedule... Tomorrow you have 5 appointments, including 3 personal training sessions and 2 prospect tours. Shall I retrieve the details for the 10 AM session?


## Installation & Usage

To install and use the **ClubPlanner** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clubplanner](https://vinkius.com/mcp/clubplanner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
