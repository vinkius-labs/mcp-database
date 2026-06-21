# Cobot MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cobot)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cobot-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cobot-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage coworking spaces via Cobot — track memberships, monitor bookings, and manage resources directly from any AI agent.

## Description
Connect your **Cobot** account to any AI agent and take full control of your coworking space management through natural conversation. Streamline how you manage members, resources, and billing natively.

### What you can do

- **Membership Oversight** — List and retrieve details for all active memberships including their names and plan details natively
- **Booking Intelligence** — Access and monitor resource bookings within specific date ranges flawlessly
- **Resource Management** — List all bookable resources like desks and meeting rooms flawlessly
- **Booking Lifecycle** — Create new bookings for resources directly from your chat interface securely
- **Invoicing Logistics** — List and review membership invoices and their payment status flawlessly
- **Space Visibility** — Retrieve core information and metadata about your coworking space directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Cobot Access Token and Space Subdomain
3. Start managing your coworking space from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Space Managers** — monitor daily bookings and membership status using natural language
- **Community Managers** — audit member rosters and resource availability without opening the dashboard
- **Accountants** — quickly look up invoice status and payment history straight from their chat interface
- **Ops Teams** — verify resource configurations and monitor space metadata


## Available Tools
- **create_new_booking**: Create a new booking for a resource
- **get_membership_details**: Get detailed information for a specific membership
- **get_cobot_space_info**: Retrieve core information and metadata about the coworking space
- **list_space_bookings**: List all resource bookings within a specific date range
- **list_cobot_invoices**: List all membership invoices and their payment status
- **list_cobot_memberships**: List all active memberships in the coworking space
- **list_membership_plans**: List all available membership plans in the space
- **list_space_resources**: List all bookable resources (desks, rooms) in the space


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cobot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active memberships in my coworking space."

**🤖 AI Agent:**
> Retrieving active memberships... I found 25 members across various plans: 10 'Full-time Desk', 12 'Part-time 10 Days', and 3 'Enterprise Suites'. Would you like the details for any specific member?

---

**👤 You:**
> "Show me the bookings for 'Large Meeting Room' for this week."

**🤖 AI Agent:**
> Checking bookings for the Large Meeting Room... There are 4 reservations this week: Monday at 10 AM, Wednesday at 2 PM, and two on Friday morning.

---

**👤 You:**
> "Are there any unpaid invoices from last month?"

**🤖 AI Agent:**
> Checking account history... I found 2 unpaid invoices from last month for members 'Sarah Smith' and 'Global Tech'. All other memberships are in good standing.


## Installation & Usage

To install and use the **Cobot** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cobot](https://vinkius.com/mcp/cobot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
