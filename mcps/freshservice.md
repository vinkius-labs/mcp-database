# Freshservice MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freshservice)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Manage your IT service desk, track tickets, and oversee assets via AI agents with Freshservice.

## Description
Connect your **Freshservice** instance to any AI agent to automate your IT Service Management (ITSM) operations through the Model Context Protocol (MCP). Freshservice is an intelligent, right-sized ITSM solution that empowers enterprises to modernize IT and other business functions. This MCP server enables you to track IT tickets, manage your CMDB asset inventory, and retrieve detailed requester profiles directly through natural conversation.

### Key Features

- **Ticket Orchestration** — List all service desk tickets, fetch detailed metadata including priority and status, and open new IT incidents instantly.
- **Asset Management (CMDB)** — Access your IT hardware and software asset inventory to maintain full context of your infrastructure.
- **Workforce Insights** — List all IT agents and requesters (employees) to understand workloads and verify contact details.
- **Change & Problem Tracking** — Monitor change requests and problem records to ensure IT stability and compliance.
- **Release Management** — Access IT release records to coordinate software deployments effectively.
- **Department Oversight** — List company departments configured in the ITSM platform to optimize ticket routing.
- **Real-time Synchronization** — Keep your IT operations data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Freshservice Domain prefix and API Key (found in your Profile Settings)
3. Start managing your IT service desk from Claude, Cursor, or any MCP client

### Who is this for?

- **IT Managers** — quickly check incident volumes or change request statuses without manual dashboard navigation.
- **Service Desk Agents** — get a real-time overview of ticket details and requester profiles via simple AI commands.
- **System Administrators** — automate the retrieval of asset metadata and release records seamlessly.


## Available Tools
- **create_itsm_ticket**: Open an IT ticket
- **check_itsm_status**: Verify helpdesk status
- **get_asset_details**: Get asset metadata
- **get_requester_details**: Get user metadata
- **get_ticket_details**: Get ticket metadata
- **list_support_agents**: List IT agents
- **list_it_assets**: List IT assets
- **list_change_requests**: List IT changes
- **list_it_problems**: List problem records
- **list_it_releases**: List release records
- **list_requesters**: List end-users
- **list_itsm_tickets**: List IT tickets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freshservice** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active IT tickets in my service desk."

**🤖 AI Agent:**
> Retrieving tickets... I found 5 active incidents, including 'VPN Access Failure' (Priority: High) and 'Software Request' (Priority: Low). Would you like the full details for the VPN issue?

---

**👤 You:**
> "Show me the details for requester 'Jane Smith'."

**🤖 AI Agent:**
> Searching requesters... I found Jane Smith (jane@example.com). She is in the 'Engineering' department and has 2 open IT tickets associated with her profile.

---

**👤 You:**
> "Create a new IT ticket: 'Printer Not Working' from 'johndoe@email.com'."

**🤖 AI Agent:**
> Ticket created! I have successfully opened incident ID 98765 regarding 'Printer Not Working' for johndoe@email.com. It is currently in the 'Open' status.


## ❓ FAQ

**Q: How do I get an API Key for Freshservice?**
Log in to your Freshservice instance, click on your Profile picture in the top-right corner, go to 'Profile Settings', and your API Key will be displayed on the right side.

**Q: What is my 'Domain prefix'?**
Your domain prefix is the first part of your Freshservice URL (e.g. if your URL is 'acme.freshservice.com', the prefix is 'acme').

**Q: Can I view my CMDB assets via the agent?**
Yes! Use the 'list_it_assets' tool to retrieve your hardware and software inventory from the Freshservice CMDB.

**Q: Is it possible to track change management requests?**
Yes, the 'list_change_requests' tool allows you to monitor all change tickets to ensure proper IT governance and stability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freshservice](https://vinkius.com/mcp/freshservice)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Freshservice** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `freshservice` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Freshservice** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "freshservice": {
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
