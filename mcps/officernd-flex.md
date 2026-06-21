# OfficeRnD Flex MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/officernd-flex)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Manage flexible workspaces via OfficeRnD — track members, bookings, and billing directly from your AI agent.

## Description
Connect your **OfficeRnD Flex** account to your AI agent and streamline your coworking or flexible workspace operations through natural conversation using their powerful Developer API.

### What you can do

- **Member Oversight** — List all registered members and retrieve detailed profile information and membership statuses.
- **Booking Management** — Access active and historical bookings for meeting rooms, desks, and other workspace resources.
- **Resource Intelligence** — List all bookable assets in your workspace and monitor their availability.
- **Contract Tracking** — View all membership and resource usage contracts to stay on top of commitments.
- **Billing & Payments** — Access a history of all generated invoices and monitor received payments in real-time.
- **Plan Management** — List all available membership and billing plans defined in your organization.
- **Deep Inspection** — Fetch complete metadata for specific members, bookings, or teams using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your OfficeRnD Client ID, Client Secret, and Organization ID
3. Start managing your workspace from Claude, Cursor, or any MCP client

### Who is this for?

- **Community Managers** — quickly check if a member has a valid contract or verify today's room bookings.
- **Operations Leads** — monitor resource usage and billing statuses directly from your workspace.
- **Office Admins** — automate the retrieval of member lists and invoice data for daily reporting.


## Available Tools
- **get_booking_details**: Get specific booking details
- **get_member_details**: Get specific member info
- **list_bookings**: List resource bookings
- **list_member_contracts**: List member contracts
- **list_billing_invoices**: List billing invoices
- **list_members**: List workspace members
- **list_billing_payments**: List received payments
- **list_billing_plans**: List membership plans
- **list_workspace_resources**: List available resources
- **list_teams**: List workspace teams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OfficeRnD Flex** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active bookings for today."

**🤖 AI Agent:**
> Retrieving bookings... I found 8 reservations for today, including 'Conference Room A' (10:00 AM - 12:00 PM), 3 hot desks, and 4 other meeting spaces. Would you like the member details for the Conference Room A booking?

---

**👤 You:**
> "Show me the details for member ID 'mem_98765'."

**🤖 AI Agent:**
> Inspecting member mem_98765... This belongs to 'John Smith'. He is a 'Dedicated Desk' member since 2022, associated with the 'Innovate Tech' team. His account is currently 'Active'. Shall I list his active contracts?

---

**👤 You:**
> "List our available billing plans."

**🤖 AI Agent:**
> Retrieving billing plans... You have 5 active plans defined: 'Hot Desk Monthly', 'Dedicated Desk', 'Private Office Small', 'Enterprise Custom', and 'Virtual Office'. Would you like the price and terms for the Hot Desk plan?


## ❓ FAQ

**Q: How do I get my OfficeRnD API credentials?**
Log in to your OfficeRnD Flex portal and navigate to Settings > Developer Tools > Applications to create a new client and generate your ID and Secret.

**Q: Can I see real-time room availability?**
Yes! Use the `list_bookings` tool to see current and upcoming reservations, and `list_workspace_resources` to see the full list of bookable assets.

**Q: What is the Organization ID in OfficeRnD?**
The Organization ID is a unique identifier for your OfficeRnD instance, often found in your portal's URL or in the general settings tab.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/officernd-flex](https://vinkius.com/mcp/officernd-flex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OfficeRnD Flex** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `officernd-flex` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OfficeRnD Flex** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "officernd-flex": {
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
