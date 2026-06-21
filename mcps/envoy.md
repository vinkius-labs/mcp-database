# Envoy MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/envoy)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/envoy-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/envoy-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage workplace operations via Envoy — register visitors, book desks and rooms, track deliveries, and monitor office capacity directly from any AI agent.

## Description
Connect your **Envoy** workplace account to any AI agent and take full control of your office management and visitor registration through natural conversation.

### What you can do

- **Visitor Orchestration** — Register expected arrivals and deliver QR code invites seamlessly while mapping NDA tracking and security compliance natively
- **Hot Desk Management** — List all available desks and reserve physical workspace elements by committing exact timing payloads directly into the organizational map
- **Meeting Room Control** — Identify bookable rooms and spaces, calculating maximal volumetric tracking and reporting integration limits securely
- **Logistical Tracking** — Monitor incoming deliveries and package states, extracting pickup receipts and bypassing front desk barriers flawlessly
- **Office Capacity Auditing** — Measure real-time occupancy metrics and compute active relational loads to ensure workplace compliance bounding
- **Employee Presence Monitoring** — Analyze specific HR identity connections fetching log trails to validate physical office sign-ins across any date range
- **Location Navigation** — Iterate through global office locations and workspaces to parse precise geographic configurations and maximum capacity limits

### How it works

1. Subscribe to this server
2. Enter your Envoy API Key (found in Envoy Console > Integrations > API)
3. Start managing your workplace operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Office Managers** — manage visitor lists and desk reservations without opening the Envoy dashboard
- **Executive Assistants** — pre-register guests and book meeting rooms using natural language
- **Logistics Teams** — monitor package deliveries and coordinate office sign-ins in real-time
- **Security Teams** — audit office capacity and verify employee presence through natural conversation


## Available Tools
- **list_locations**: List all office locations managed in Envoy
- **list_visitors**: List all visitors checked in or expected at an Envoy location
- **pre_register_visitor**: Pre-register a visitor in Envoy
- **list_deliveries**: List all deliveries at an Envoy location
- **list_desks**: List all hot desks at an Envoy location
- **reserve_desk**: Reserve a hot desk in Envoy
- **cancel_desk_reservation**: Cancel an Envoy desk reservation
- **list_rooms**: List all bookable rooms/spaces at an Envoy location
- **get_employee_signins**: Get employee sign-in data for an Envoy location
- **get_capacity**: Get real-time capacity data for an Envoy location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Envoy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Pre-register guest 'Jane Doe' (jane@example.com) for tomorrow at 10 AM"

**🤖 AI Agent:**
> Guest registered! I've scheduled Jane Doe's arrival at your office for tomorrow at 10:00 AM. A QR code invite and NDA link have been sent to her email. Would you like to reserve a meeting room for this time?

---

**👤 You:**
> "Reserve desk 'D-101' at the 'Main Office' for next Friday"

**🤖 AI Agent:**
> Desk reserved! You have successfully booked desk D-101 for next Friday. Your reservation is confirmed in the Envoy organizational map and will appear on your office dashboard.

---

**👤 You:**
> "What is the current occupancy at the London office?"

**🤖 AI Agent:**
> Checking London capacity... There are currently 45 people checked in out of a 100-person limit (45% occupancy). The office is currently within compliance boundaries.


## Installation & Usage

To install and use the **Envoy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/envoy](https://vinkius.com/mcp/envoy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
