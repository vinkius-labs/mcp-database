# ClubReady MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clubready)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/clubready-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/clubready-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage members, check-ins, classes, billing, prospects, and staff for your ClubReady (ABC Fitness) gym through natural conversation.

## Description
Connect your **ClubReady** (ABC Fitness) gym to any AI agent and manage your fitness facility through natural conversation.

### What you can do

- **Members** — Search by name, email, barcode, or phone. View profiles and membership status
- **Check-ins** — Track daily check-ins, validate memberships, and trigger door access
- **Billing** — Check balances, payment status, past-due amounts, and auto-pay settings
- **Classes** — View group fitness schedule, capacity, and instructor assignments
- **Rosters** — List members registered for specific classes with check-in status
- **Prospects** — Manage sales pipeline: leads, sources, and assigned salespeople
- **Staff** — List trainers, front desk, and managers with roles and certifications
- **Membership Plans** — Browse all tiers: monthly, annual, student, family, corporate

### Who is this for?

- **Gym Owners (30K+ locations)** — Instant member insights and revenue data
- **Front Desk** — Quick member check-in, barcode scanning, and account lookup
- **Sales Teams** — Prospect pipeline, lead tracking, and conversion metrics
- **Franchise Operators** — Multi-location oversight with Chain ID support
- **Collections** — Past-due accounts, billing status, and payment recovery


## Available Tools
- **search_members**: Returns profile, membership status, billing status, and check-in history. Used by 30K+ gym locations.

Search gym members
- **list_membership_plans**: Includes pricing, billing frequency, and initiation fee.

List membership plans
- **get_store_info**: Get gym location info
- **get_member**: Get member profile
- **get_member_billing**: Critical for collections.

Get member billing status
- **list_check_ins**: Shows member name, time, barcode scanned, and membership type. Filter by date.

List gym check-ins
- **do_check_in**: Validates membership status, records the visit, and triggers door access. Returns success/failure with reason.

Check in a member
- **list_schedule**: Filter by date range.

List class schedule
- **list_class_roster**: Shows check-in status, waitlist position, and membership used.

List class roster
- **list_prospects**: Essential for gym sales teams.

List sales prospects
- **list_staff**: Includes role, certifications, and contact info.

List gym staff


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ClubReady** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check in member John Smith at the front desk."

**🤖 AI Agent:**
> ✅ **Check-in successful!**

👤 **John Smith** (ID: 45231)
🏷️ Barcode: CR-2024-45231
📋 Plan: Premium All-Access ($89/month)
✅ Status: Active — Paid through April 30
🔓 Door access: Granted
📊 Visit #47 this year (avg 3.8x/week)

John is one of your most engaged members!

---

**👤 You:**
> "Show me the roster for the 6 PM Advanced Cycling class."

**🤖 AI Agent:**
> Here is the roster for 6 PM Advanced Cycling with Trainer Sarah: 14 members booked out of 20 spots. 3 members have already checked in. Waitlist is currently empty.

---

**👤 You:**
> "List all members with past-due billing balances over $50."

**🤖 AI Agent:**
> Scanning billing database... Found 8 members with overdue balances exceeding $50. Top flagged accounts: Michael R. ($150 past due), Emma W. ($89 past due). Shall I send automated reminders?


## Installation & Usage

To install and use the **ClubReady** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clubready](https://vinkius.com/mcp/clubready)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
