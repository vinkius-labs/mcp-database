# PushPress MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pushpress)
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


## Available Tools (8)
- **list_plans**: Includes pricing and billing cycle.

List membership plans
- **list_appointments**: List PT appointments
- **list_messages**: List sent messages
- **list_webhooks**: List active webhooks
- **search_customers**: Returns profile, active plan, check-in count, and billing status.

Search gym members
- **get_customer**: Get member profile
- **list_checkins**: List gym check-ins
- **list_classes**: List scheduled classes


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


## ❓ FAQ

**Q: Does PushPress have a TypeScript SDK?**
Yes! PushPress provides an early-alpha TypeScript SDK on GitHub, and their v3 API is the most modern in the gym management space.

**Q: Does PushPress integrate with external waiver systems?**
PushPress has a robust internal waiver and document signing system, but its API can also sync status with external CRM and waiver platforms.

**Q: Can I use the API to book an appointment for a client?**
Yes, the v3 API allows authorized agents to schedule personal training sessions and appointments dynamically based on coach availability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pushpress](https://vinkius.com/mcp/pushpress)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PushPress** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pushpress` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PushPress** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pushpress": {
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
