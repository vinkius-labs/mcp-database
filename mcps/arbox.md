# Arbox MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arbox)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/arbox-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/arbox-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Manage members, schedule, coaches, leads, payments, and CRM for your Arbox-powered fitness studio through natural conversation.

## Description
Connect your **Arbox** studio to any AI agent.

- **Members** — Search with CRM profile, engagement score, attendance
- **Schedule** — Classes with coach, spots left, enrolled members
- **Coaches** — Trainers with specialties and availability
- **Leads** — Sales pipeline: source, status, assigned salesperson
- **Memberships** — Unlimited, limited, punch cards, trials
- **Payments** — Transaction tracking, amounts, methods
- **Products** — Retail: merchandise, supplements, accessories

Arbox is a CRM-first studio management platform popular in Israel and growing globally. Its strength is in lead management and sales pipeline tracking.


## Available Tools
- **search_members**: Returns profile, membership, attendance, and engagement score.

Search studio members
- **get_member**: Get member profile
- **list_schedule**: List class schedule
- **list_memberships**: List membership plans
- **list_coaches**: List coaches/trainers
- **list_leads**: Key for studio sales pipeline.

List sales leads
- **list_payments**: List payments
- **list_products**: List products/retail
- **get_branch_info**: Get branch info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Arbox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me our active leads and their status."

**🤖 AI Agent:**
> Active sales pipeline:

🔥 **Hot leads (3)**:
- Sarah M. — Trial class booked for tomorrow, source: Instagram
- Mike T. — Visited twice, interested in monthly plan
- Ana R. — Referred by member Lisa, wants personal training

🟡 **Warm leads (5)**:
- 3 from website form, 2 from walk-ins

🔵 **Cold leads (8)**:
- Last contact > 14 days ago

Conversion rate this month: 42% (8/19 leads converted)


## Installation & Usage

To install and use the **Arbox** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arbox](https://vinkius.com/mcp/arbox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
