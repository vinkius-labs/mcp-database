# MakePlans MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/makeplans-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/makeplans-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/makeplans-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Online booking and appointment scheduling via MakePlans MCP.

## Description
Connect your MakePlans account to your AI agent. Manage bookings, list services, check staff availability, and create appointments directly using natural language.


## Available Tools
- **create_booking**: Create a new booking
- **delete_booking**: Delete/Cancel a booking
- **get_booking**: Get details for a specific booking
- **get_resource**: Get details for a specific resource
- **get_service**: Get details for a specific service
- **list_bookings**: List all bookings in MakePlans
- **list_people**: List people (staff)
- **list_resources**: g., rooms, equipment).

List resources
- **list_services**: g., "Consultation", "Haircut").

List available services
- **list_available_slots**: List available time slots for a service


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MakePlans** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my bookings for this month."

**🤖 AI Agent:**
> I've fetched your bookings. You have 3 appointments this month: 'Consultation' on the 12th, 'Follow-up' on the 15th, and 'Review' on the 20th.

---

**👤 You:**
> "What services are available for booking?"

**🤖 AI Agent:**
> Currently, you offer 2 services: 'General Consultation' (ID: 101) and 'Advanced Therapy' (ID: 102).

---

**👤 You:**
> "Show available slots for service ID '123'."

**🤖 AI Agent:**
> I found 4 available slots for service '123' today, starting from 14:00 to 17:00 at 1-hour intervals.


## Installation & Usage

To install and use the **MakePlans** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/makeplans-alternative](https://vinkius.com/mcp/makeplans-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
