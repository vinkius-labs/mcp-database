# Everbridge Critical Management MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/everbridge-critical-management)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Equip your AI agent to manage critical notifications, track incidents, and monitor contacts via the Everbridge API.

## Description
Integrate **Everbridge**, the leader in critical event management (CEM), directly into your AI workflow. Manage your organization's emergency notifications and broadcasts, track active and historical incidents, monitor contact repositories and distribution groups, and oversee your crisis response using natural language.

### What you can do

- **Notification Oversight** — List and retrieve detailed information, subjects, and delivery statuses for all your critical broadcasts.
- **Incident Intelligence** — Monitor active and historical incidents, resolving severity levels, timelines, and response logs.
- **Contact Management** — Access and monitor your organization's contact repository and distribution groups, resolving communication methods and group IDs.
- **Crisis Auditing** — Retrieve high-level summaries of incident volume, notification delivery success, and organizational crisis health instantly.

### How it works

1. Connect the Everbridge integration to your AI assistant.
2. Authorize using your Everbridge Organization ID, API Username, and API Password.
3. Orchestrate your critical event management and emergency communication strategy through intuitive conversation.

### Who is this for?

- **Crisis Managers** — Quickly check notification statuses and incident timelines on the go.
- **Emergency Operations Teams** — Research contact groups and distribution lists via chat during active events.
- **Safety & Security Teams** — Monitor organization-wide crisis metadata and response metrics instantly.


## Available Tools
- **get_everbridge_org_metadata**: Retrieve metadata and limits for your Everbridge organization
- **get_contact_profile_and_methods**: Get detailed profile and communication methods for a specific contact
- **get_incident_detailed_data**: Get detailed settings and timeline for a specific critical incident
- **get_notification_detailed_status**: Get detailed delivery status and statistics for a specific notification
- **quick_crisis_event_audit**: Retrieve a high-level summary of active incidents and recent notifications
- **list_critical_contacts**: List all contacts registered in your Everbridge organization
- **list_contact_distribution_groups**: List all contact distribution groups configured in your organization
- **list_high_severity_incidents**: Identify incidents that are currently flagged with high severity (mock logic)
- **list_critical_incidents**: List all active and historical critical incidents
- **list_critical_notifications**: List all critical notifications and broadcasts sent via Everbridge


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Everbridge Critical Management** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active critical incidents."

**🤖 AI Agent:**
> I've found 2 active incidents: 'Building Fire - North Wing' (Severity: High) and 'System Outage - HQ' (Severity: Medium). Would you like to see the notification history for the Building Fire?

---

**👤 You:**
> "Check delivery status for notification ID '1234567'."

**🤖 AI Agent:**
> Notification ID '1234567' (Subject: Weather Warning) was sent to 500 contacts. 485 were successfully delivered (97%) and 120 contacts have confirmed receipt. Should I list the contacts who haven't confirmed yet?

---

**👤 You:**
> "Show me the contact details for 'John Doe'."

**🤖 AI Agent:**
> John Doe (External ID: 998877) has 3 communication methods: Mobile (SMS/Call), Work Email, and Personal Phone. They are a member of the 'Emergency Response Team' group. Would you like the full profile for this contact?


## ❓ FAQ

**Q: How do I get Everbridge API credentials?**
You need your **Organization ID** (found in your Everbridge dashboard URL), along with a dedicated **API Username** and **Password** created by your organization's administrator. Ensure the user has the 'API' role assigned.

**Q: Can the agent launch new notifications?**
This integration currently focuses on listing and auditing notifications, contacts, and incidents. Launching actual emergency broadcasts should be managed via the Everbridge manager portal or mobile app to ensure safety protocols are followed.

**Q: Does the integration show confirmation rates?**
Yes, you can use the get_notification_detailed_status tool to retrieve detailed delivery statistics, including how many contacts received and confirmed the notification.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/everbridge-critical-management](https://vinkius.com/mcp/everbridge-critical-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Everbridge Critical Management** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `everbridge-critical-management` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Everbridge Critical Management** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "everbridge-critical-management": {
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
