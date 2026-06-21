# Bookeo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bookeo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bookeo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bookeo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage bookings, customers, products, payments, and availability for your Bookeo-powered fitness or activity business through natural conversation.

## Description
Connect your **Bookeo** account to any AI agent and manage your booking-based business through natural conversation.

### What you can do

- **Bookings** — View reservations with participants, pricing, and payment status
- **Products** — Browse all bookable products: classes, sessions, tours, rentals
- **Customers** — Search clients, view profiles, and booking history
- **Payments** — Track revenue, payment methods, and refunds
- **Availability** — Check real-time available slots for any product
- **Business** — Access your business profile, timezone, and configuration
- **Webhooks** — Monitor active event notifications

### Who is this for?

- **Fitness Studios** — Class bookings, capacity management, and payments
- **Activity Centers** — Tour bookings, rental reservations, and group management
- **Personal Trainers** — Appointment scheduling and client tracking
- **Wellness Providers** — Service bookings and availability management


## Available Tools
- **list_bookings**: Includes participant count, time, product, price, and payment status. Filter by date range.

List bookings and reservations
- **get_booking**: Get booking details
- **list_products**: Includes pricing, duration, and capacity.

List bookable products
- **search_customers**: Returns profile, booking history, and preferences.

Search customers
- **get_customer**: Get customer profile
- **list_payments**: Filter by date for revenue analysis.

List payments
- **check_availability**: Essential for real-time booking assistance.

Check available time slots
- **get_business_info**: Get business info
- **list_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bookeo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Are there any open slots for yoga tomorrow?"

**🤖 AI Agent:**
> Available yoga slots tomorrow:

🧘 **7:00 AM** Sunrise Yoga — 4 spots left (6/10)
🧘 **10:00 AM** Gentle Flow — 8 spots left (2/10)
🧘 **5:30 PM** Power Yoga — 2 spots left (8/10) ⚡
🧘 **7:00 PM** Yin Yoga — 6 spots left (4/10)

The 5:30 PM Power Yoga is almost full — only 2 spots remaining!

---

**👤 You:**
> "Extract the customer profile and booking history for Alice Smith."

**🤖 AI Agent:**
> Profile fetched. Alice Smith joined 8 months ago. She holds 15 past bookings consisting mostly of Pilates sessions, and has completed all mandatory payments. No future classes booked.

---

**👤 You:**
> "Check total revenue collected for today's classes."

**🤖 AI Agent:**
> Calculating via Bookeo Payments matrix. Today's sessions collected $1,450.00 across 33 unique participants and 4 scheduled classes.


## Installation & Usage

To install and use the **Bookeo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bookeo](https://vinkius.com/mcp/bookeo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
