# Mindbody MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mindbody)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mindbody-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mindbody-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage classes, appointments, clients, staff, and sales from your Mindbody-powered fitness studio, spa, or wellness business through natural conversation.

## Description
Connect your **Mindbody** business to any AI agent and run your fitness studio, spa, or wellness center through natural conversation.

### What you can do

- **Classes** — View schedules, class types, upcoming sessions, and instructor assignments
- **Appointments** — Browse booked appointments, check staff availability, and manage private sessions
- **Clients** — Search members, view visit history, check memberships, and track attendance patterns
- **Staff** — List instructors and therapists with bios, certifications, and assigned services
- **Sales** — Track revenue, view transactions, browse retail products, and check pricing options
- **Site** — Access business details, multiple locations, and session types
- **Enrollments** — Monitor multi-week courses, workshops, and teacher training programs

### Who is this for?

- **Studio Owners** — Get instant business insights, revenue summaries, and attendance trends
- **Front Desk Staff** — Search clients, check schedules, and answer member questions instantly
- **Fitness Managers** — Monitor class fill rates, instructor performance, and member retention
- **Multi-Location Operators** — Compare performance across all your locations in one conversation


## Available Tools
- **get_client_history**: Shows attendance patterns, no-shows, and engagement over time. Critical for retention analysis.

Get client visit history
- **get_client_memberships**: Shows remaining visits, expiration dates, and auto-pay status.

Get client memberships and packages
- **get_site_info**: Get studio/business info
- **list_appointments**: ) with client name, staff, time, duration, and status. Filter by date range or staff member.

List booked appointments
- **list_class_schedules**: Useful for understanding the studio's regular weekly cadence.

List recurring class schedules
- **list_class_types**: g. Vinyasa Yoga, CrossFit WOD, Spin). Includes name, category, description, and duration.

List all class types/descriptions
- **list_classes**: Filter by date range or class type. Essential for seeing the studio schedule at a glance.

List scheduled classes
- **list_enrollments**: Includes dates, capacity, pricing, and enrolled clients.

List course enrollments
- **list_locations**: Includes address, phone, tax rates, and operating hours.

List studio locations
- **list_products**: Includes name, price, category, and inventory count.

List retail products
- **list_sales**: Includes amount, payment method, client, and date. Essential for revenue tracking.

List sales transactions
- **list_services_pricing**: Shows price, session count, and expiration policy.

List services and pricing options
- **list_staff**: Includes name, bio, photo URL, certifications, and assigned services.

List all staff and instructors
- **list_staff_schedule**: Useful for viewing availability, managing bookings, or planning coverage.

Get a staff member's appointment schedule
- **search_clients**: Returns demographics, contact info, account balance, and membership status. The core CRM tool for studio owners.

Search studio clients/members


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mindbody** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What classes are available this week?"

**🤖 AI Agent:**
> This week at your studio:

📅 **Monday**: Vinyasa Flow 7:00 AM (Sarah, 15/20 spots), Power Yoga 6:00 PM (Mike, 12/18 spots)
📅 **Tuesday**: CrossFit WOD 6:30 AM (Jake, FULL), Spin 5:30 PM (Ana, 8/25 spots)
📅 **Wednesday**: Pilates Reformer 9:00 AM (Lisa, 4/10 spots), Hot Yoga 7:00 PM (Sarah, 18/25 spots)

The Tuesday CrossFit is already full — would you like me to check the waitlist?

---

**👤 You:**
> "How much revenue did we make this month?"

**🤖 AI Agent:**
> Revenue for March 2026:

💰 **Total**: $47,320
- Memberships: $28,400 (60%)
- Class Packs: $9,850 (21%)
- Personal Training: $5,200 (11%)
- Retail: $3,870 (8%)

That's 12% above February ($42,250). Your new 'Unlimited Yoga' membership is your top seller with 23 new sign-ups this month.

---

**👤 You:**
> "Show me clients who haven't visited in the last 30 days."

**🤖 AI Agent:**
> Found 47 members with no visits in the last 30 days:

⚠️ **High risk** (active membership, no visits):
- Jessica M. — Unlimited, last visit Feb 8 (54 days ago)
- David K. — 10-class pack (7 remaining), last visit Feb 15
- Amanda R. — Monthly, last visit Feb 21

These 3 members represent $450/month in at-risk revenue. Consider a re-engagement campaign?


## Installation & Usage

To install and use the **Mindbody** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mindbody](https://vinkius.com/mcp/mindbody)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
