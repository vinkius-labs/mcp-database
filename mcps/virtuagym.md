# Virtuagym MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/virtuagym)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Manage members, events, trainers, memberships, nutrition plans, and workout programs for your Virtuagym club through natural conversation.

## Description
Connect your **Virtuagym** club to any AI agent.

- **Members** — Search, profiles, body metrics, fitness progress
- **Events** — Group classes with trainer and capacity
- **Activities** — Class types: yoga, spinning, CrossFit, swimming
- **Trainers** — Personal trainers with specialties
- **Memberships** — Plans with pricing and contracts
- **Nutrition Plans** — Meal plans and dietary tracking (unique to Virtuagym)
- **Workout Plans** — Training programs with exercises and progression

Virtuagym is Europe's leading gym management platform, also offering corporate wellness and nutrition tracking — features no competitor matches.


## Available Tools
- **search_members**: Returns profile, membership, check-in history, and fitness progress.

Search gym members
- **get_member**: Get member profile
- **list_events**: List classes/events
- **list_activities**: With description and duration.

List activity types
- **list_memberships**: List membership plans
- **list_trainers**: List trainers
- **list_nutrition_plans**: Unique to Virtuagym.

List nutrition plans
- **list_workout_plans**: List workout plans
- **get_club_info**: Get club info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Virtuagym** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the profile for Thomas Miller and see what his current workout routine is."

**🤖 AI Agent:**
> Fetching member details ('get_member')...
Thomas Miller (ID: 7721):
- Status: Active (Pro Membership)
- Current Program: 'Hypertrophy Phase 2' (Assigned by Trainer Dave)
- Recent Activity: Checked in yesterday at 5:30 PM
- Body Metrics: Last weigh-in 82kg (Down 2kg this month).

---

**👤 You:**
> "List all group classes running tomorrow morning."

**🤖 AI Agent:**
> tomorrow morning's classes ('get_schedule'):
- 07:00 AM: HIIT Bootcamp with Sarah (12/15 booked)
- 08:30 AM: Morning Vinyasa Yoga with Elena (8/20 booked)
- 10:00 AM: Spinning Masterclass with Marcus (20/20 FULL)
Would you like me to book a member into any of these?


## ❓ FAQ

**Q: What makes Virtuagym unique?**
Virtuagym uniquely combines gym management with built-in nutrition tracking, workout programming, and corporate wellness — features no other platform offers in one solution. It's the market leader in Europe, particularly in the Netherlands, Germany, and Spain.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/virtuagym](https://vinkius.com/mcp/virtuagym)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Virtuagym** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `virtuagym` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Virtuagym** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "virtuagym": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
