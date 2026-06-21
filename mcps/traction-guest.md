# Traction Guest MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/traction-guest)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage visitor operations via Traction Guest — list hosts, locations, invites, sign-ins, and group visits directly from any AI agent.

## Description
Connect your **Traction Guest** (now Sign In Enterprise) account to any AI agent and take full control of visitor management workflows through natural conversation.

### What you can do

- **Host Management** — List, create, and batch-create hosts (employees) who receive and host visitors
- **Location Management** — List all office locations and inspect their configuration details
- **Invite Management** — Create, read, update, and delete visitor invites for scheduled arrivals
- **Sign-in Tracking** — List and manage visitor check-ins, monitor who is currently on-site
- **Group Visits** — Create and manage group appointments like tours, training sessions, and interviews
- **Security Watchlists** — List and create watchlists for visitor screening
- **Audit Logging** — Access audit logs for compliance and security tracking
- **Registration Management** — List pre-registered visitors and manage registration queues

### How it works

1. Subscribe to this server
2. Enter your Traction Guest API key from the developer portal
3. Start managing visitor operations from Claude, Cursor, or any MCP-compatible client

No more navigating the Traction dashboard for every visitor action. Your AI acts as a dedicated receptionist or security coordinator.

### Who is this for?

- **Reception Teams** — instantly create invites, check in visitors, and manage group appointments without opening the Traction dashboard
- **Security Staff** — monitor who is on-site, check watchlists, and review audit logs for compliance
- **Facility Managers** — track visitor activity across multiple locations and manage host assignments
- **HR Teams** — batch-create hosts for new employees and manage interview/tour scheduling


## Available Tools
- **create_group_visit**: Provide group data as JSON including name, scheduled date, expected attendees, host, and location.
Example: { "name": "Campus Tour", "scheduledDate": "2026-04-15", "expectedAttendees": 15, "hostId": "host_123", "locationId": "loc_456" }

Create a new group visit (group appointment)
- **create_host**: Hosts are employees who can receive and host visitors.
You must provide host data as JSON including name, email, department, and optionally phone number and location assignment.
Example: { "firstName": "John", "lastName": "Doe", "email": "john@company.com", "department": "Engineering" }

Create a new host (employee) in Traction Guest
- **create_hosts_batch**: Provide an array of host objects as JSON. Each host must include firstName, lastName, and email.
This is useful for bulk onboarding new employees or importing host lists from HR systems.
Example: [{ "firstName": "John", "lastName": "Doe", "email": "john@company.com" }, { "firstName": "Jane", "lastName": "Smith", "email": "jane@company.com" }]

Create multiple hosts in a single batch operation
- **create_invite**: You must provide the location_id
and invite data as JSON including visitor name, email, host, and scheduled date/time.
Example: { "firstName": "Alice", "lastName": "Johnson", "email": "alice@example.com", "hostId": "host_123", "scheduledDate": "2026-04-10", "scheduledTime": "10:00" }

Create a new visitor invite for a location
- **create_signin**: Provide sign-in data as JSON including visitor information, host, location, and purpose of visit.
Example: { "visitorName": "Alice Johnson", "hostId": "host_123", "locationId": "loc_456", "purpose": "Interview" }

Create a new visitor sign-in (check-in a visitor on-site)
- **create_watchlist**: Provide watchlist data as JSON including name, description, and optionally entries.
Example: { "name": "Restricted Visitors", "description": "Individuals not permitted on-site" }

Create a new security watchlist
- **delete_group_visit**: You must provide the group_visit_id.
This action cannot be undone. Use this to cancel scheduled group events that are no longer needed.

Delete a group visit
- **delete_invite**: You must provide the invite_id.
This action cannot be undone. Use this to cancel scheduled visits that are no longer needed.
Be careful as this will remove all associated visitor data for that invite.

Delete a visitor invite
- **get_group_visit**: Use the group_visit_id obtained from list_group_visits to inspect full group visit details.

Get detailed information about a specific group visit
- **get_invite**: Use the invite_id obtained from list_invites to inspect full invite details.

Get detailed information about a specific visitor invite
- **get_location**: Use the location_id obtained from list_locations to inspect full location details.
This is useful for verifying location configuration before creating invites or managing visitors.

Get detailed information about a specific location
- **get_signin**: Use the signin_id obtained from list_signins to inspect full visit details.

Get detailed information about a specific visitor sign-in
- **list_audit_logs**: Use this for compliance reporting, security investigations, and operational auditing.

List audit logs for compliance and security tracking
- **list_group_visits**: Each group visit includes name, scheduled date, expected attendees, host, and location.
Use this to manage tours, training sessions, interviews, and other group events.

List all group visits (group appointments) in your organization
- **list_hosts**: Each host includes name, email, department, location assignment, and contact information.
Use this to see who is available to host visitors and verify host assignments to locations.

List all hosts (employees/hosts) in your Traction Guest organization
- **list_invites**: Each invite includes visitor name, email, host, scheduled date, location, and status.
Use this to see upcoming visitors, manage invite lists, and prepare for expected arrivals.
Optionally provide a location_id to filter invites for a specific location.

List all visitor invites in your organization
- **list_locations**: Each location includes name, address, timezone, and configuration details.
Use this to discover available locations before creating invites, sign-ins, or assigning hosts.

List all locations in your Traction Guest organization
- **list_packages**: Each package includes name, description, included features, and pricing.
Use this to understand available visitor management configurations.

List packages (visitor management packages/plans) in your organization
- **list_registrations**: Each registration includes visitor information, registration date, and associated event or purpose.
Use this to manage pre-registration queues and convert registrations to invites.

List visitor registrations in your organization
- **list_signins**: Each sign-in includes visitor name, host, location, check-in time, check-out time, and purpose of visit.
Use this to monitor visitor activity, track who is currently on-site, and review visit history.

List all visitor sign-ins (check-ins) in your organization
- **list_watchlists**: Watchlists are used to screen visitors against known individuals who should be flagged or denied access.
Each watchlist includes name, description, and number of entries.
Use this to verify security screening configurations.

List all security watchlists in your organization
- **update_group_visit**: Common updates include rescheduling,
changing expected attendee count, or updating host assignments. You must provide the group_visit_id
and the fields to update as JSON.

Update an existing group visit
- **update_invite**: You must provide the invite_id
and the fields to update as JSON. Common updates include rescheduling dates, changing hosts,
or updating visitor information. Only provide the fields you want to change.

Update an existing visitor invite
- **update_signin**: Common updates include recording check-out times,
updating visit purpose, or modifying host assignments. You must provide the signin_id
and the fields to update as JSON.

Update an existing visitor sign-in record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Traction Guest** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all upcoming visitor invites for the New York office this week."

**🤖 AI Agent:**
> I found 8 upcoming invites for the New York office:
1. **Alice Johnson** — Host: John Smith — April 10, 10:00 AM — Interview
2. **Bob Williams** — Host: Sarah Davis — April 10, 2:00 PM — Client Meeting
3. **Carol Martinez** — Host: Mike Brown — April 11, 9:30 AM — Vendor Demo
4. **David Lee** — Host: John Smith — April 12, 11:00 AM — Interview
5. **Emma Wilson** — Host: Sarah Davis — April 13, 3:00 PM — Training Session
6. **Frank Garcia** — Host: Mike Brown — April 13, 4:00 PM — Delivery
7. **Grace Taylor** — Host: John Smith — April 14, 10:00 AM — Interview
8. **Henry Anderson** — Host: Sarah Davis — April 14, 1:00 PM — Partner Meeting

Would you like to create a new invite or check current sign-ins?

---

**👤 You:**
> "Create a group visit for a Campus Tour on April 20th with 20 expected attendees, hosted by Sarah Davis at the Main Office."

**🤖 AI Agent:**
> I've successfully created the group visit:
- **Group Visit ID**: GV-20260420-001
- **Name**: Campus Tour
- **Date**: April 20, 2026
- **Expected Attendees**: 20
- **Host**: Sarah Davis
- **Location**: Main Office

The group visit is now scheduled and ready for individual invite creation. Would you like me to create invites for specific attendees?

---

**👤 You:**
> "Show me who is currently checked in at the New York office and list any security watchlist alerts."

**🤖 AI Agent:**
> Currently checked in at New York office:
1. **Alice Johnson** — Checked in: 9:15 AM — Host: John Smith — Purpose: Interview — Badge: V-1234
2. **Bob Williams** — Checked in: 1:45 PM — Host: Sarah Davis — Purpose: Client Meeting — Badge: V-1235
3. **Carol Martinez** — Checked in: 2:00 PM — Host: Mike Brown — Purpose: Vendor Demo — Badge: V-1236

✅ **Security Watchlists**: No alerts detected. All current visitors have passed security screening.

Would you like to check in a new visitor or review audit logs?


## ❓ FAQ

**Q: How do I get a Traction Guest API key and where do I find it?**
Log in to your Traction Guest account, go to the **Developer Portal** at us.tractionguest.com/dev_portal, and generate a new API key. Copy the key immediately and paste it into the API key field below. This key authenticates all API v3 requests to https://us.tractionguest.com/api/v3.

**Q: What's the difference between invites, sign-ins, and registrations?**
**Invites** are scheduled visitor appointments created in advance (future visits). **Sign-ins** are actual check-in records when visitors arrive on-site (current/past visits). **Registrations** are pre-registration records awaiting conversion to invites. The workflow is: Registration → Invite → Sign-in (check-in) → Sign-out.

**Q: Can I create multiple hosts at once for bulk employee onboarding?**
Yes! Use the `create_hosts_batch` tool with an array of host objects. Each host needs firstName, lastName, and email. This is much more efficient than creating hosts one at a time, especially when onboarding new teams or importing from HR systems.

**Q: How do I manage group visits like tours and training sessions?**
Use `create_group_visit` to schedule a group event with name, date, expected attendees, host, and location. Then use `list_group_visits` to see all upcoming group events. You can update or delete group visits as needed. Each group visit tracks expected vs actual attendance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/traction-guest](https://vinkius.com/mcp/traction-guest)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Traction Guest** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `traction-guest` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Traction Guest** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "traction-guest": {
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
