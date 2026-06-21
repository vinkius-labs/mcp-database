# Everfit Coaching MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/everfit-coaching)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/everfit-coaching-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/everfit-coaching-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage coaching clients, track workout plans, and monitor performance via the Everfit API.

## Description
Integrate **Everfit**, the leading software platform for fitness coaches and personal trainers, directly into your AI workflow. Manage your client database and profile details, track workout plans and session completions, monitor daily tasks and habit tracking, and oversee your coaching operation using natural language.

### What you can do

- **Client Oversight** — List and retrieve detailed profiles, fitness metrics, and subscription status for all your coaching clients.
- **Workout Intelligence** — Monitor assigned workout plans and routines, resolving exercise lists and real-time completion statuses.
- **Habit Management** — Access and monitor daily tasks and habit tracking, ensuring your clients stay on track with their wellness goals.
- **Coaching Auditing** — Retrieve high-level summaries of client volume, program diversity, and organizational coaching health instantly.

### How it works

1. Connect the Everfit integration to your AI assistant.
2. Authorize using your Everfit API Key (found in your business settings).
3. Orchestrate your fitness coaching and client management strategy through intuitive conversation.

### Who is this for?

- **Fitness Coaches** — Quickly check client progress and workout completions on the go.
- **Gym Owners** — Research trainer caseloads and organizational coaching metadata via chat.
- **Operations Teams** — Monitor client engagement and active subscription counts instantly.


## Available Tools
- **get_everfit_account_metadata**: Retrieve metadata and limits for your Everfit business account
- **get_client_performance_metrics**: Get high-level performance and health metrics for a client
- **get_client_detailed_profile**: Get detailed profile and fitness metrics for a specific client
- **quick_coaching_volume_audit**: Retrieve a high-level summary of clients, programs, and active trainers
- **list_currently_active_clients**: Identify clients who are currently in an "Active" coaching status
- **list_client_daily_tasks**: List all daily tasks and habit tracking for a specific client
- **list_coaching_clients**: List all clients managed in your Everfit coaching account
- **list_coaching_programs**: List all coaching programs and templates available in your account
- **list_coaching_trainers**: List all trainers and coaching staff in your organization
- **list_client_workout_plans**: List all workout plans and assigned routines for a specific client


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Everfit Coaching** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active coaching clients."

**🤖 AI Agent:**
> I've found 12 active clients, including 'John Miller' and 'Alice Connor'. 8 clients have completed their workout today. Would you like to see the profile details for John Miller?

---

**👤 You:**
> "Show me the workout plan for 'Alice Connor'."

**🤖 AI Agent:**
> Alice Connor has an active '12-Week Transformation' program. Today's routine is 'Upper Body Power'. It includes 8 exercises, including Bench Press and Pull-ups. Should I pull the completion status for this session?

---

**👤 You:**
> "What are the performance metrics for client ID 'CUST-12345'?"

**🤖 AI Agent:**
> For client ID 'CUST-12345', I've retrieved the metrics: 10,500 average daily steps, 7.5 hours of sleep, and 4 workouts completed this week. Their weight has decreased by 2kg this month. Would you like to see the detailed step trend?


## Installation & Usage

To install and use the **Everfit Coaching** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/everfit-coaching](https://vinkius.com/mcp/everfit-coaching)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
