# Glofox MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/glofox)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/glofox-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/glofox-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage members, classes, trainers, bookings, and purchases for your Glofox-powered gym or fitness studio through natural conversation.

## Description
Connect your **Glofox** gym or studio to any AI agent and manage your fitness business through natural conversation.

### What you can do

- **Members** — Search and view member profiles, membership status, and attendance
- **Classes** — Browse scheduled group classes with capacity and trainer info
- **Courses** — Monitor multi-week programs, challenges, and bootcamps
- **Trainers** — List coaches with specialties and certifications
- **Bookings** — Track class reservations, check-ins, and waitlists
- **Memberships** — View all plans: basic, premium, VIP, student, corporate
- **Purchases** — Track member spending on memberships, PT, and retail

### Who is this for?

- **Gym Owners** — Instant member insights, class fill rates, and revenue data
- **Fitness Managers** — Trainer schedules, class performance, and retention metrics
- **Front Desk** — Quick member lookup, booking status, and account info


## Available Tools
- **search_members**: Returns profile, membership status, check-in history, and account balance. The core CRM of your gym.

Search gym members
- **get_member**: Get member details
- **list_classes**: Filter by date to see a specific day.

List scheduled classes
- **list_courses**: Shows sessions, pricing, and enrollment.

List multi-week courses
- **list_memberships**: Includes pricing, access hours, and perks.

List membership plans
- **list_trainers**: List trainers and coaches
- **list_bookings**: Shows who booked which class, check-in status, and waitlist.

List class bookings
- **list_purchases**: Filter by member for individual spending.

List member purchases


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Glofox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many active members do we have?"

**🤖 AI Agent:**
> Active member summary:

👥 **Total active**: 847 members
- Premium Unlimited: 312 (37%)
- Basic 3x/week: 298 (35%)
- Student: 142 (17%)
- Corporate: 95 (11%)

📈 Net growth: +23 this month (31 new, 8 cancellations)

---

**👤 You:**
> "Who is teaching the HIIT bootcamp tomorrow morning?"

**🤖 AI Agent:**
> The HIIT bootcamp scheduled for tomorrow at 7:00 AM (Studio 1) will be taught by Coach Marcus Davies. The class is currently 85% full with 17 out of 20 spots booked.

---

**👤 You:**
> "Show me all overdue payments for this week."

**🤖 AI Agent:**
> There are currently 6 members with overdue membership payments totaling $450 this week. Would you like me to list their contact details so the Front Desk can follow up?


## Installation & Usage

To install and use the **Glofox** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/glofox](https://vinkius.com/mcp/glofox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
