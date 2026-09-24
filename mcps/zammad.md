# Zammad MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/zammad)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Automate helpdesk workflows via Zammad — manage tickets, users, and organizations directly from any AI agent.

## Description
Connect your **Zammad** helpdesk to any AI agent to streamline your customer support and user management through natural conversation.

### What you can do

- **Ticket Management** — List, retrieve, and create tickets to stay on top of customer requests using `list_tickets` and `get_ticket`.
- **User & Organization Control** — Search, create, and update user profiles and organizational data with tools like `search_users` and `list_organizations`.
- **Group & Role Insights** — List and search through system groups and roles to understand permissions and assignments.
- **Data Privacy** — Securely handle user deletions via specialized data privacy tasks using `data_privacy_delete_user`.

### How it works

1. Subscribe to this server
2. Enter your Zammad URL and Personal Access Token
3. Start managing your helpdesk from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Leads** — quickly get ticket statuses and user history without switching tabs.
- **System Admins** — manage users, groups, and organizations directly from the terminal or AI interface.
- **DevOps Engineers** — integrate helpdesk data into automated workflows and reporting.


## Available Tools (41)
- **get_links**: Supply the object type and its unique ID.

Get links for a specific object
- **update_ticket**: You must specify the ticket ID.

Update an existing Zammad ticket
- **list_organizations**: List all Zammad organizations
- **summarize_ticket**: Provide the target ticket ID.

Trigger async generation of a ticket summary
- **create_ticket_article**: Always specify the target Ticket ID.

Create a new article on a ticket
- **create_ticket**: Must provide a title and either a group or customer.

Create a new Zammad ticket
- **data_privacy_delete_user**: Use this method instead of direct deletion. Provide the User ID.

Delete a user via Data Privacy task (Recommended over direct delete)
- **get_me**: Get current Zammad user details
- **get_shared_draft**: Pass the specific ticket ID.

Get shared draft for a ticket
- **get_ticket_article**: Use the unique Article ID.

Get details for a specific ticket article
- **list_calendars**: List calendars
- **list_ticket_articles**: Supply the required Ticket ID.

List articles for a specific ticket
- **list_tickets**: Use filters to narrow the search results.

List Zammad tickets
- **list_users**: List all Zammad users
- **search_groups**: The query must contain group-identifying keywords.

Search for groups in Zammad
- **add_tag**: Provide both the object type and the object ID.

Add a tag to an object
- **create_user**: Supply all required user details.

Create a new Zammad user
- **delete_ticket**: Provide the unique Ticket ID for deletion.

Delete a Zammad ticket
- **delete_user**: Specify the target User ID.

Delete a Zammad user
- **get_group**: Provide the required Group ID.

Get details for a specific Zammad group
- **get_organization**: Provide the required Organization ID.

Get details for a specific Zammad organization
- **get_ticket**: Provide a valid Ticket ID.

Get details for a specific Zammad ticket
- **get_user**: Provide the required User ID.

Get details for a specific Zammad user
- **list_all_tags**: List all tags in the system (Admin)
- **list_checklist_items**: List checklist items
- **list_checklists**: List checklists
- **list_checklist_templates**: List checklist templates
- **list_groups**: List all Zammad groups
- **list_mentions**: List mentions
- **list_roles**: Do not specify any filters when calling this tool.

List all Zammad roles
- **list_slas**: List SLAs
- **list_tags_for_object**: Provide both the object type and its ID.

List tags for a specific object (e.g., Ticket)
- **list_ticket_priorities**: List ticket priorities
- **list_ticket_states**: List ticket states
- **list_time_accountings**: You must provide the ticket ID.

List time accountings for a ticket
- **remove_tag**: You must provide the object type and object ID.

Remove a tag from an object
- **search_organizations**: The query must contain organization-identifying keywords.

Search for organizations in Zammad
- **search_roles**: The query must contain role-identifying keywords.

Search for roles in Zammad
- **search_tickets**: The query must contain ticket-identifying keywords.

Search for tickets in Zammad
- **search_users**: The query must contain user-identifying keywords.

Search for users in Zammad
- **update_user**: Include the target User ID.

Update an existing Zammad user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zammad** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active tickets in Zammad."

**🤖 AI Agent:**
> I've retrieved the tickets. You have 3 open tickets, including 'Login Issue' (ID: 101) and 'Billing Inquiry' (ID: 102). Would you like to see the details for any of these?

---

**👤 You:**
> "Search for a user with the email 'customer@example.com'."

**🤖 AI Agent:**
> Searching... I found one user matching that email: Jane Doe (User ID: 505). She is currently assigned to the 'Premium Customers' organization.

---

**👤 You:**
> "Get the details for ticket ID 42."

**🤖 AI Agent:**
> Inspecting ticket 42... The subject is 'Server Downtime', created by Mark Smith. The current state is 'open' and it is assigned to the 'Technical Support' group.


## ❓ FAQ

**Q: Can I search for specific users or organizations within Zammad?**
Yes! You can use the `search_users` and `search_organizations` tools to find specific records using search queries directly from your AI agent.

**Q: How do I safely delete a user according to data privacy standards?**
It is recommended to use the `data_privacy_delete_user` tool. This initiates a Data Privacy task in Zammad, which is the preferred method over direct deletion for compliance.

**Q: Can I view my own Zammad profile details?**
Yes, the `get_me` tool allows you to retrieve the profile details of the currently authenticated user associated with your access token.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/zammad](https://vinkius.com/en/ai-agent-connect/zammad)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zammad** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zammad` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zammad** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zammad": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
