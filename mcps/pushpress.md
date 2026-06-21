# PushPress MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pushpress)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pushpress-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pushpress-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-management](../categories/business-management.md)

Manage members, check-ins, classes, plans, and appointments for your PushPress gym through natural conversation.

## Description
Connect your **PushPress** gym to any AI agent.

- **Members** — Search, profiles, billing
- **Check-ins** — Daily visits with method tracking
- **Classes** — Group classes with coach and capacity
- **Plans** — Memberships, punch cards, trials
- **Appointments** — PT and private coaching
- **Messages** — Emails, push, SMS
- **Webhooks** — Real-time event notifications

Built for CrossFit boxes, independent gyms, and S&C facilities.


## Available Tools
- **search_customers**: Returns profile, active plan, check-in count, and billing status.

Search gym members
- **get_customer**: Get member profile
- **list_checkins**: List gym check-ins
- **list_classes**: List scheduled classes
- **list_plans**: Includes pricing and billing cycle.

List membership plans
- **list_appointments**: List PT appointments
- **list_messages**: List sent messages
- **list_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PushPress** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many people checked in today?"

**🤖 AI Agent:**
> Today's check-ins: 47 total. Peak: 6-7 AM (14). By method: App 28, Kiosk 15, Manual 4. +6 vs last week.

---

**👤 You:**
> "Who is enrolled in the 6 AM CrossFit class today?"

**🤖 AI Agent:**
> The 6 AM CrossFit class has 12 members enrolled: John D., Sarah M., Michael T... There are 3 spots remaining.

---

**👤 You:**
> "Which members have a billing issue right now?"

**🤖 AI Agent:**
> Currently, 4 members have failed payments or expired credit cards on file. I have generated a detailed list so you can follow up.


## Installation & Usage

To install and use the **PushPress** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pushpress](https://vinkius.com/mcp/pushpress)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
