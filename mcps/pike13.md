# Pike13 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pike13)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Manage classes, clients, staff, invoices, visits, and analytics for your Pike13-powered fitness studio through natural conversation.

## Description
Connect your **Pike13** studio to any AI agent and manage your fitness business through natural conversation.

### What you can do

- **Events** — View scheduled classes and sessions with instructors, capacity, and enrollment
- **Clients** — Search members by name, email, or phone with detailed profiles
- **Staff** — List instructors with roles, certifications, and class assignments
- **Plans** — Browse membership plans, class packs, and drop-in pricing
- **Invoices** — Track revenue, payments, refunds, and financial reporting
- **Visits** — Analyze check-in records for retention and engagement analytics
- **Business** — Access account profile and configuration

### Why Pike13?

Pike13 uniquely offers a **Reporting API** with deep analytics — making it the best choice for data-driven studio owners who want AI-powered business intelligence. Combined with the Core API and Webhooks, it provides the most comprehensive data access in the fitness industry.


## Available Tools
- **list_events**: Filter by date range. Follows JSON:API 1.0 spec.

List scheduled classes/events
- **get_event**: Get event details
- **search_people**: Returns profiles, active plans, visit count, and account balance.

Search clients/members
- **get_person**: Get person profile
- **list_staff**: List staff members
- **list_plans**: Includes pricing and visit limits.

List service plans
- **list_invoices**: Filter by date for financial reporting.

List invoices and revenue
- **list_visits**: Key data for retention analytics.

List member visits
- **get_business_info**: Get business account info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pike13** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's our revenue this month?"

**🤖 AI Agent:**
> Revenue report — March 2026:

💰 **Total revenue**: $24,580
- Memberships: $18,200 (74%)
- Drop-ins: $3,100 (13%)
- PT sessions: $2,480 (10%)
- Retail: $800 (3%)

📊 **142 invoices** processed, 97% collection rate
📈 **vs. February**: +8% ($22,760 → $24,580)
👥 **12 new members** this month

Top revenue day: Saturday March 15 ($1,420)

---

**👤 You:**
> "List the staff members teaching yoga classes tomorrow."

**🤖 AI Agent:**
> Tomorrow's Yoga instructors: Sarah Jenkins (Vinyasa flow, 9 AM), David Lee (Ashtanga, 12 PM), and Emily Chen (Restorative, 6 PM).

---

**👤 You:**
> "How many new clients bought a membership this week?"

**🤖 AI Agent:**
> This week, 8 new clients successfully purchased an active membership plan, representing a 15% increase compared to the previous week.


## ❓ FAQ

**Q: Does Pike13 support real-time webhooks?**
Yes! Pike13 has a dedicated Webhooks API that sends real-time notifications for events like new clients, invoice changes, and new visits. This MCP server focuses on the Core and Reporting APIs for querying data.

**Q: Can I query staff payroll data?**
Through the Reporting API, you can query staff hours, class assignments, and pay rates to calculate or audit your payroll.

**Q: What payment gateways are supported?**
Pike13 typically integrates with Stripe, Evo, and other major gateways to process credit card and ACH payments directly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pike13](https://vinkius.com/mcp/pike13)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pike13** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pike13` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pike13** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pike13": {
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
