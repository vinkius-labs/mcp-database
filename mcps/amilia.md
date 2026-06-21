# Amilia MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amilia)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/amilia-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/amilia-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Recreation and activity management — manage programs, accounts, and registrations via AI.

## Description
Connect your **Amilia (SmartRec)** account to your AI agent to unlock professional recreation management and participant orchestration. From auditing activity programs and monitoring attendance to managing household accounts and tracking registrations, your agent handles your community operations through natural conversation.

### What you can do

- **Program & Activity Orchestration** — List and manage recreational programs, activities, and specific class occurrences
- **Account & Contact Oversight** — Retrieve detailed profiles for families/households and their individual contacts
- **Registration Tracking** — Audit sign-ups and retrieve registration histories for specific accounts
- **Attendance Management** — Retrieve rosters and check-in statuses for specific event occurrences
- **Operational Insights** — Quickly identify popular activities or retrieve attendance reports directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Amilia Organization Identifier, Username, and Password
3. Start managing your recreation programs and monitoring attendance through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recreation Directors** — automate program audits and monitor activity popularity effortlessly
- **Facility Managers** — quickly look up class occurrences and attendance rosters on the fly
- **Customer Support Teams** — retrieve family account details and registration histories to resolve inquiries
- **Administrators** — track sign-ups and manage community engagement using simple commands


## Available Tools
- **list_accounts**: List family accounts
- **get_account_details**: Get account profile
- **list_contacts**: List account contacts
- **list_programs**: g. Summer Camp, Fall Sessions).

List recreational programs
- **get_program_details**: Get program metadata
- **list_activities**: List program activities
- **list_activity_occurrences**: List activity schedules
- **list_registrations**: List account registrations
- **get_attendance**: Get attendance roster


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amilia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active programs in my organization."

**🤖 AI Agent:**
> I've retrieved your programs. You have 3 active programs: 'Summer Camp 2026', 'Fall Swimming Lessons', and 'Adult Fitness'. Would you like to see the activities scheduled under the Summer Camp program?

---

**👤 You:**
> "Show me the contacts associated with account ID 'acc_12345'."

**🤖 AI Agent:**
> I've retrieved the contacts for the Smith Household (Account acc_12345). There are 3 contacts: John Smith (Parent), Mary Smith (Parent), and Timmy Smith (Child). Would you like to check their recent registration history?

---

**👤 You:**
> "Get the attendance roster for occurrence ID 'occ_98765'."

**🤖 AI Agent:**
> I've retrieved the roster for the 'Beginner Yoga' session scheduled for today at 10:00 AM. There are 15 registered participants, and currently, 12 have checked in. I've listed the names of the missing participants for you.


## Installation & Usage

To install and use the **Amilia** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amilia](https://vinkius.com/mcp/amilia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
