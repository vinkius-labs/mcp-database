# Apptoto MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apptoto)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage appointments and messaging with Apptoto — track events, contacts, and bookings via AI.

## Description
The **Apptoto MCP Server** connects your AI agent to your appointment scheduling and automated messaging platform. Streamline your calendar management, monitor client interactions, and track online bookings using simple natural language.

### Key Features

- **Appointment Management** — List all upcoming and historical events, and retrieve full metadata for any specific appointment.
- **Contact Oversight** — Access and search your client database, including names, phone numbers, and email addresses.
- **Booking Tracking** — Monitor online bookings and check availability for new appointments directly from your chat.
- **Messaging Lists** — Manage your opt-in and opt-out lists for automated SMS and email reminders.
- **Account Verification** — Quickly check your API connection and account status using secure API keys.
- **Workflow Integration** — Create new events and link them to your existing contacts and messaging sequences.

### Who is this for?

- **Service Professionals** — Quickly check your daily schedule and client details without switching between apps.
- **Office Managers** — Monitor booking trends and ensure all clients are receiving automated reminders.
- **Sales Teams** — Track appointments and follow up with leads directly from your AI workspace.


## Available Tools (8)
- **create_event**: Create a new appointment event
- **get_account_check**: Verify Apptoto account connection
- **get_contact**: Get details for a specific contact
- **get_event**: Get details for a specific event
- **list_bookings**: List all online bookings
- **list_contacts**: List all contacts in Apptoto
- **list_events**: List all appointment events
- **list_lists**: List all opt-in/opt-out messaging lists


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apptoto** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my appointments for today."

**🤖 AI Agent:**
> I've retrieved your schedule for today. You have 4 appointments, including 'Consultation with John Smith' at 10:00 AM and 'Follow-up Call' at 2:00 PM.

---

**👤 You:**
> "Find contact details for 'Jane Doe'."

**🤖 AI Agent:**
> I've found Jane Doe in your contacts. Her phone number is (555) 123-4567 and her email is jane.doe@example.com.

---

**👤 You:**
> "Create a new appointment 'Site Audit' for tomorrow at 9 AM."

**🤖 AI Agent:**
> The appointment 'Site Audit' has been successfully created for tomorrow at 9:00 AM.


## ❓ FAQ

**Q: How do I find my Apptoto API Key?**
Log in to Apptoto, go to **Settings > API**, and you will find your API Key there. If you don't see it, contact Apptoto support.

**Q: Can I create new appointments via the API?**
Yes, you can use the `create_event` tool to add new appointments to your Apptoto calendar. Provide the subject, start time, and end time.

**Q: Does Apptoto support two-way messaging?**
Yes, Apptoto supports two-way SMS and email messaging. While this server focuses on event and contact management, the contacts you retrieve feed into your messaging workflows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apptoto](https://vinkius.com/mcp/apptoto)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Apptoto** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `apptoto` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Apptoto** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apptoto": {
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
