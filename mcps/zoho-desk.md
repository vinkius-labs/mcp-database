# Zoho Desk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-desk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

AI-powered helpdesk: manage tickets, contacts, and support workflows via agents.

## Description
### What you can do

Transform your Zoho Desk into an AI-ready support powerhouse. Your agents can now autonomously:

- **List and search tickets** across all departments with keyword filters
- **Create, update, and assign tickets** with proper priority and status management
- **Manage contacts and accounts** for complete customer relationship context
- **Add public replies and internal notes** for seamless team collaboration
- **Review departments and agents** for optimal resource allocation
- **Track ticket lifecycle** from Open to Closed with full audit history

### How it works

1. **Connect your Zoho Desk account** via OAuth token from the Zoho API Console
2. **Provide your Organization ID** (found in Zoho Desk setup)
3. **Ask your AI agent** to manage support operations naturally
4. **No coding required** — the MCP server handles all API complexity

### Who is this for?

Perfect for **customer support teams**, **IT helpdesks**, and **SaaS companies** using Zoho Desk. Empower AI agents to handle tier-1 support, triage tickets, escalate issues, and maintain customer records — all through natural language commands. Ideal for teams managing 100+ tickets daily who want to reduce response times and automate repetitive workflows.


## Available Tools (13)
- **add_note**: Notes are only visible to agents and not visible to customers. Use this for internal collaboration, escalation notes, or context that should not be shared with the customer. Requires a valid ticket ID.

Add an internal note to a Zoho Desk ticket
- **add_reply**: The reply is visible to the customer via email and in the customer portal. Commonly used by agents to respond to customer inquiries. The reply is sent as HTML format. Requires a valid ticket ID.

Add a reply to a Zoho Desk ticket
- **create_contact**: Requires firstName, lastName, and email. Optionally set phone, title, department, account association, and custom fields. Returns the created contact data including the new contact ID.

Create a new contact in Zoho Desk
- **create_ticket**: Requires at minimum a subject, contact ID, and department ID. Optionally set priority (Low, Medium, High, Urgent), status, classification, and custom fields. Returns the created ticket data including the new ticket ID.

Create a new support ticket in Zoho Desk
- **get_contact**: Use this to review customer details before interacting with their tickets.

Get details of a specific Zoho Desk contact
- **get_ticket**: Use this to review full ticket history before responding.

Get details of a specific Zoho Desk ticket
- **list_accounts**: Returns account name, industry, website, and associated contacts. Useful for B2B support to understand which company a contact belongs to.

List accounts (organizations) in Zoho Desk
- **list_agents**: Returns agent name, email, role, and availability status. Use this to find available agents for ticket assignment or escalation. Requires a valid department ID.

List agents in a Zoho Desk department
- **list_contacts**: Returns contact name, email, phone, and account association. Useful for customer lookup before creating tickets or reviewing customer history.

List contacts (customers) in Zoho Desk
- **list_departments**: Departments are used to categorize tickets and assign agents. Each department has a unique ID needed for ticket creation and agent listing. Use this first to get department IDs.

List all departments in Zoho Desk
- **list_tickets**: Useful for agents to review open, pending, or resolved tickets across all departments. Returns ticket ID, subject, status, priority, and assignee.

List all support tickets in Zoho Desk
- **search_tickets**: Searches subject, description, and custom fields. Use this to find tickets related to a specific topic, customer name, or product. Returns matching tickets with basic info.

Search tickets in Zoho Desk by keyword
- **update_ticket**: Commonly used to change ticket status from Open to Closed or to reassign to another agent. Only pass the fields you want to update.

Update an existing Zoho Desk ticket


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho Desk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all open high-priority tickets from the Support department"

**🤖 AI Agent:**
> I'll search for high-priority open tickets in your Support department right away.

---

**👤 You:**
> "Create a new ticket for john@example.com about billing issue with subject 'Payment Failed'"

**🤖 AI Agent:**
> I'll create the billing ticket and assign it to the appropriate department.

---

**👤 You:**
> "Add a public reply to ticket #12345 saying 'We are investigating your issue and will update you shortly'"

**🤖 AI Agent:**
> I'll post the reply to the ticket right now.


## ❓ FAQ

**Q: What Zoho Desk plan do I need for this MCP server?**
This MCP server works with any paid Zoho Desk plan (Standard, Professional, Enterprise). The free plan has limited API access. Ensure your organization has API enabled in admin settings.

**Q: Can this MCP server automate ticket routing and escalation?**
Yes! AI agents can list tickets, filter by status/priority, update assignees, change departments, and add internal notes for escalation. Combined with workflow rules in Zoho Desk, you can build fully automated support pipelines.

**Q: Does this work with Zoho's multi-tenant organizations?**
Absolutely. The MCP server requires an orgId parameter, so you can connect to any Zoho Desk organization you have access to. For multiple orgs, deploy separate MCP instances with different credentials.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-desk](https://vinkius.com/mcp/zoho-desk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zoho Desk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zoho-desk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zoho Desk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zoho-desk": {
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
