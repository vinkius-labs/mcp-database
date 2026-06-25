# Arbox MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arbox-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Run your fitness studio or gym with member management, class scheduling, and payment processing in one connected platform.

## Description
Connect your **Arbox** account to any AI agent and take full control of your fitness business management and automated lead engagement workflows through natural conversation.

### What you can do

- **Client & Lead Orchestration** — List and manage your active member directory programmatically, or create new high-fidelity lead profiles directly from your chat interface
- **Class Schedule Intelligence** — Access your high-fidelity class schedules and available training sessions in real-time to coordinate member bookings perfectly
- **Administrative Task Management** — Programmatically create follow-ups and operational tasks for your front-desk staff to ensure a perfectly coordinated facility
- **Relationship Intelligence** — Retrieve complete high-fidelity profiles for any client or prospect to maintain a perfectly coordinated relationship ecosystem
- **Operational Monitoring** — Access organization-level metadata and verify account connectivity directly through your agent for instant performance reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Arbox dashboard (Settings > Integrations)
3. Start orchestrating your fitness studio's growth from Claude, Cursor, or any MCP client

No more manual logging of walk-in leads or digging through complex session calendars. Your AI acts as your dedicated studio administrator and sales coordinator.

### Who is this for?

- **Gym & Studio Owners** — instantly retrieve upcoming class summaries and manage staff tasks using natural language commands
- **Sales & Front Desk** — automate the ingestion of new leads and monitor membership health without leaving your workspace
- **Developers** — integrate high-speed fitness CRM data into custom member applications through simple AI queries


## Available Tools (14)
- **book_class**: Book a class
- **check_arbox_status**: Verify connectivity
- **create_client**: Create a member
- **create_lead**: Create a lead
- **create_task**: Create a task
- **get_client**: Get member details
- **get_lead**: Get lead details
- **get_schedule**: Get schedule
- **list_classes**: List classes
- **list_clients**: List members
- **list_memberships**: List memberships
- **list_tasks**: List tasks
- **update_client**: Update a member
- **list_leads**: List leads


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Arbox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active clients in my Arbox member directory."

**🤖 AI Agent:**
> I've retrieved your member directory. You currently have 150 active clients, including @user1 and @user2. Would you like the detailed membership metadata for any of them?

---

**👤 You:**
> "Show the class schedule for today."

**🤖 AI Agent:**
> Accessing schedule... Today you have 8 sessions, including 'HIIT Training' at 5 PM and 2 'Yoga Flow' classes. One session is currently fully booked. Shall I retrieve the attendee metadata for the 5 PM class?

---

**👤 You:**
> "Create a new lead 'John Doe' (john@example.com) and set a follow-up task."

**🤖 AI Agent:**
> Lead orchestrated! I've successfully created the profile for John Doe (ID: lead_123) and registered a high-fidelity follow-up task for your team. He is now active in your sales funnel. Need any other CRM actions?


## ❓ FAQ

**Q: How do I find my Arbox API Key?**
Log in to your account, navigate to **Settings** > **Integrations**, and copy your unique API Key from the credentials section.

**Q: Can I add a walk-in lead via AI?**
Yes! The `create_arbox_lead` tool allows your agent to register new prospects by providing their contact details programmatically.

**Q: How do I check today's class schedule?**
Use the `get_arbox_schedule` tool to retrieve a high-fidelity list of all upcoming sessions and training blocks for the current day.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arbox-alternative](https://vinkius.com/mcp/arbox-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Arbox** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `arbox-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Arbox** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "arbox-alternative": {
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
