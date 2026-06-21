# meetergo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/meetergo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/meetergo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/meetergo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Schedule meetings intelligently with routing rules that send leads to the right rep based on territory, availability, and deal size.

## Description
Connect your **meetergo** account to any AI agent and take full control of your scheduling orchestration and appointment management through natural conversation. meetergo provides a robust platform for managing team availability and customer bookings, and this integration allows you to retrieve booking metadata, monitor team schedules, and manage meeting templates directly from your chat interface.

### What you can do

- **Booking & Appointment Orchestration** — List all scheduled meetings and retrieve detailed metadata programmatically to ensure your calendar is always synchronized.
- **Availability & Schedule Intelligence** — Access and monitor team member availabilities directly from the AI interface to track throughput and identify open slots.
- **Template & Type Control** — List and retrieve all active meeting templates (meeting types) via natural language to facilitate frictionless meeting coordination.
- **User & Context Oversight** — Access granular details for specific users and their configured settings using simple AI commands to maintain a clear overview of your digital infrastructure.
- **Operational Monitoring** — Track system responses and manage booking metadata to ensure your scheduling pipelines are always optimized.

### How it works

1. Subscribe to this server
2. Enter your meetergo API Key (starts with ak_live:) and User ID from your dashboard settings
3. Start managing your scheduling from Claude, Cursor, or any MCP-compatible client

No more manual status checking in the dashboard for new bookings. Your AI acts as a dedicated scheduling coordinator or office assistant.

### Who is this for?

- **Client-facing Teams** — quickly retrieve booking summaries and coordinate meetings without switching apps.
- **Operations Managers** — automate the retrieval of team availability and track appointment loads via natural conversation.
- **Developers** — integrate real-time scheduling data and booking intelligence directly within the chat.


## Available Tools
- **cancel_booking**: Cancel a booking
- **check_meetergo_status**: Verify connectivity
- **create_booking**: Create a booking
- **get_availability**: Get user availability
- **get_booking**: Get booking details
- **get_me**: Get my profile
- **get_meeting_type**: Get meeting type
- **get_user**: Get user details
- **list_availability**: List availability
- **list_bookings**: List bookings
- **list_meeting_types**: List meeting types
- **list_users**: List users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **meetergo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active bookings in meetergo."

**🤖 AI Agent:**
> I've retrieved your bookings. You have 5 active appointments including 'Product Demo' and 'Support Call'. Which one would you like to see attendee details for?

---

**👤 You:**
> "What meeting templates do I have?"

**🤖 AI Agent:**
> I've retrieved your meeting types. You have 3 templates configured: '30 Min Discovery', 'Technical Deep-dive', and 'Onboarding session'.

---

**👤 You:**
> "Check my availability in meetergo."

**🤖 AI Agent:**
> I've retrieved your availability schedules. You are currently set for 'Standard Business Hours' with exceptions for next Friday.


## Installation & Usage

To install and use the **meetergo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meetergo](https://vinkius.com/mcp/meetergo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
