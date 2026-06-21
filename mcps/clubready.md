# ClubReady MCP Server

Manage members, check-ins, classes, billing, prospects, and staff for your ClubReady (ABC Fitness) gym through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/clubready)

## Overview
**Category:** human-resources
**Tools Count:** 11

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


## Installation & Usage

To install and use the **ClubReady** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clubready](https://vinkius.com/mcp/clubready)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
