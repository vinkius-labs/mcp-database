# WellnessLiving MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wellnessliving)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wellnessliving-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wellnessliving-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage schedules, clients, staff, memberships, locations, and reports for your WellnessLiving-powered studio through natural conversation.

## Description
Connect your **WellnessLiving** studio to any AI agent and manage your fitness business through natural conversation.

### What you can do

- **Schedule** — View daily class schedule with instructors, capacity, and enrollment
- **Clients** — Search members, view profiles, credits, and attendance history
- **Staff** — List instructors and trainers with roles and schedules
- **Memberships** — Browse all promotion/membership plans with pricing
- **Locations** — Manage multi-location studios with addresses and hours
- **Reports** — Access business reports: attendance, revenue, retention
- **Business** — View account profile and configuration

### Who is this for?

- **Fitness Studios** — Full-service alternative to Mindbody with competitive pricing
- **Martial Arts Schools** — Popular in the martial arts and dance studio segment
- **Music Schools** — Used by music and performing arts schools
- **Multi-location Chains** — Consolidated reporting across all branches


## Available Tools
- **list_schedule**: List class schedule
- **search_clients**: Returns profile, memberships, and visit history.

Search clients/members
- **get_client**: Get client profile
- **list_staff**: List staff members
- **list_services**: List class types/services
- **list_memberships**: List membership plans
- **list_locations**: List business locations
- **get_report**: Reports include attendance, revenue, retention metrics.

Get business report
- **get_business_info**: Get business info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WellnessLiving** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show today's class schedule."

**🤖 AI Agent:**
> Today's schedule:

🥋 9:00 AM **Kids Karate** — Master Kim (12/15 enrolled)
🧘 10:30 AM **Yoga Flow** — Sarah (8/12 enrolled)
🥊 4:00 PM **Kickboxing** — Alex (FULL, waitlist: 2)
💃 5:30 PM **Zumba** — Maria (10/20 enrolled)
🥋 7:00 PM **Adult BJJ** — Coach Dan (14/16 enrolled)

5 classes today, 56 total registrations. Kickboxing is full — consider adding a second session?

---

**👤 You:**
> "Check David Chen's attendance history and remaining class credits."

**🤖 AI Agent:**
> Accessing client profile ('get_client_details')...
David Chen (ID: CL-992):
- Attendance: 14 visits this month (Last visit: Oct 12, Kickboxing)
- No-shows: 0
- Membership: 10-Class Pack
- Remaining Credits: 3
- Expiration: Dec 1, 2024
Would you like me to send him an email reminder to purchase a new pack?

---

**👤 You:**
> "Generate a summary of yesterday's revenue and attendance for the Uptown studio."

**🤖 AI Agent:**
> Generating daily report ('get_business_report')...
Uptown Studio - Yesterday's Summary:
- Total Revenue: $1,450.00
  - Memberships: $800.00
  - Drop-ins: $450.00
  - Merchandise: $200.00
- Total Attendance: 84 visits
- Highest utilization: 6:00 PM BJJ class (100% capacity)


## Installation & Usage

To install and use the **WellnessLiving** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wellnessliving](https://vinkius.com/mcp/wellnessliving)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
