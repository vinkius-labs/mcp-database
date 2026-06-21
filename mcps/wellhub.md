# Wellhub MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wellhub)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wellhub-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wellhub-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage employee eligibility, gym check-ins, bookings, and partner locations for your Wellhub (Gympass) corporate wellness program through natural conversation.

## Description
Connect your **Wellhub** (formerly Gympass) account to any AI agent and manage your corporate wellness program through natural conversation.

### What you can do

- **Eligibility** — Check employee eligibility, manage enrollment, and verify plan access
- **Check-ins** — Track gym visits, validate QR codes, and monitor utilization
- **Bookings** — View class reservations made through the Wellhub app
- **Classes** — List published classes visible to corporate members
- **Locations** — Manage partner gym and studio locations
- **Partner Profile** — Access business details, amenities, and network tier

### Who is this for?

- **HR Directors** — Monitor employee wellness program utilization and ROI
- **Fitness Partners** — Track Wellhub member check-ins and booking volume
- **Benefits Managers** — Verify eligibility and manage corporate wellness enrollment
- **Operations** — Real-time check-in validation and facility management


## Available Tools
- **list_eligible_employees**: Shows plan tier, activation date, and usage status.

List eligible corporate employees
- **check_eligibility**: Returns plan tier and access permissions.

Check employee eligibility
- **list_check_ins**: Shows gym name, date, time, and plan used. Essential for utilization reporting.

List gym check-ins
- **validate_check_in**: Confirms plan eligibility and records the visit. Called when a member scans their QR code at the front desk.

Validate a gym check-in
- **list_bookings**: Shows class name, time, member name, and booking status.

List class bookings
- **list_classes**: Shows schedule, capacity, and available spots visible to corporate members.

List available classes
- **get_partner_info**: Get partner profile
- **list_locations**: List partner locations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wellhub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many Wellhub check-ins did we have this week?"

**🤖 AI Agent:**
> This week's Wellhub activity:

📊 **Total check-ins**: 127
- Monday: 24 | Tuesday: 31 | Wednesday: 28 | Thursday: 22 | Friday: 15 | Weekend: 7

👥 **Unique members**: 89 (70% return rate)
📈 **vs. last week**: +12% increase

Peak time: Tuesday 6-7 PM (18 check-ins). Your most popular class for Wellhub members is the 6 PM HIIT.

---

**👤 You:**
> "Verify if Alex Johnson is eligible for the Silver tier."

**🤖 AI Agent:**
> Checking eligibility ('check_eligibility')...
Alex Johnson (Corporate ID: 99421):
- Employer: TechCorp Inc.
- Eligibility Status: Active
- Current Plan: Starter Tier
- Silver Tier Access: Yes, eligible for upgrade. Upgrade cost is $29.99/month.

---

**👤 You:**
> "List the upcoming Yoga classes available to Wellhub members at our main location."

**🤖 AI Agent:**
> Querying published classes ('get_classes')...
Upcoming Yoga at Main Studio:
1. Thu 6:00 PM - Vinyasa Flow (Wellhub Basic & above) - 4 spots left
2. Fri 7:00 AM - Morning Yoga (Wellhub Silver & above) - 10 spots left
3. Sat 9:00 AM - Power Yoga (Wellhub Gold) - Full


## Installation & Usage

To install and use the **Wellhub** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wellhub](https://vinkius.com/mcp/wellhub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
