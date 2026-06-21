# MINDBODY Health & Wellness MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mindbody-health-wellness)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage your wellness business via MINDBODY — track class schedules, client profiles, and visit history directly via AI.

## Description
Connect your AI agent to **MINDBODY**, the world's leading technology platform for the wellness industry. This integration allows you to oversee your studio operations, manage client data, and audit class schedules through natural conversation.

### What you can do

- **Schedule Management** — List and inspect upcoming class schedules, including staff assignments and times
- **Client Oversight** — Search for client profiles and retrieve detailed membership and contact information
- **Visit Tracking** — Review historical and upcoming visits for specific clients or class rosters
- **Business Intelligence** — Access site-wide information, physical locations, and available studio resources
- **Staff & Roster Auditing** — List employees and instructors to manage assignments and check class attendance
- **Transaction History** — Retrieve purchase logs for clients to track memberships and payments

### How it works

1. Subscribe to this server
2. Enter your **MINDBODY API Key** and **Site ID** (found in your MINDBODY Developer account)
3. Start managing your health and wellness operations via chat

### Who is this for?

- **Studio Owners** — quickly check daily schedules and resource availability without opening the dashboard
- **Wellness Managers** — retrieve client visit data and staff assignments for operational reporting
- **Support Teams** — lookup client membership status and purchase history to assist with inquiries


## Available Tools
- **get_class_visits**: Retrieve the list of clients attending a specific class
- **get_client_details**: Get comprehensive information for a specific client
- **get_client_purchases**: Retrieve the purchase history for a specific client
- **get_client_visits**: Retrieve the visit history for a specific client
- **get_site_info**: Retrieve information about the MINDBODY site
- **list_classes**: Retrieve the class schedule for the business
- **list_locations**: Retrieve a list of all physical locations for the business
- **list_resources**: Retrieve a list of resources (rooms, equipment) used by the business
- **list_staff**: Retrieve a list of employees/instructors for the business
- **search_clients**: Search for clients by name or email


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MINDBODY Health & Wellness** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the class schedule for today."

**🤖 AI Agent:**
> Retrieving today's schedule... You have 5 classes scheduled, starting with 'Vinyasa Flow' at 8:00 AM by Instructor Sarah.

---

**👤 You:**
> "Find the profile for client 'John Doe'."

**🤖 AI Agent:**
> Searching for 'John Doe'... I found a match! John has been a member since 2022 and has an active 'Unlimited Monthly' pass.


## ❓ FAQ

**Q: How do I find my MINDBODY Site ID?**
Your Site ID is a unique integer representing your business. You can find it in your [**MINDBODY Dashboard**](https://clients.mindbodyonline.com/) or in the emails provided during your account setup.

**Q: How do I generate an API Key?**
You must register as a developer at the [**MINDBODY Developer Portal**](https://developers.mindbodyonline.com/). Once approved, you can create a project and generate your API Key.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mindbody-health-wellness](https://vinkius.com/mcp/mindbody-health-wellness)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MINDBODY Health & Wellness** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mindbody-health-wellness` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MINDBODY Health & Wellness** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mindbody-health-wellness": {
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
