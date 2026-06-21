# Deskpro MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deskpro)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Deliver exceptional helpdesk support with ticket management, self-service portals, and SLA tracking across every channel.

## Description
Connect your **Deskpro** helpdesk to any AI agent and take full control of your customer support and internal help center workflows through natural conversation.

### What you can do

- **Ticket Orchestration** — List and manage active and archived support tickets programmatically, including monitoring message history and updating priorities in real-time
- **User & Organization Intelligence** — Access complete profiles for end-users and organizations to maintain high-fidelity records of customer relationships and account status
- **Knowledgebase Architecture** — Access and retrieve content from your help center articles programmatically to coordinate information delivery and self-service support
- **Staff Coordination** — Retrieve directories of support agents and administrators to understand team assignments and coordinate complex support routing
- **Operational Monitoring** — Check API health status, manage outbound webhooks, and monitor account metadata directly through your agent for reliable service operations

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** and **Instance URL** from your Deskpro Admin Portal (Apps & Integrations > API Keys)
3. Start managing your support pipeline from Claude, Cursor, or any MCP client

No more manual ticket shuffling or digging through help center folders. Your AI acts as your dedicated support operations and CX coordinator.

### Who is this for?

- **Support Leads & Managers** — instantly summarize ticket histories and reassign high-priority cases using natural language commands
- **Customer Success Teams** — monitor user profiles and organization health without leaving your communication tools
- **Operations Leads** — automate knowledgebase access and verify system connectivity through simple AI queries


## Available Tools (12)
- **check_api_health**: Verify Deskpro API connectivity
- **create_new_helpdesk_ticket**: Requires a subject, person email, and initial message.

Open a new support ticket
- **get_article_content**: Get details for a KB article
- **get_ticket_details**: Get details for a specific ticket
- **get_user_profile**: Get details for a specific user
- **list_helpdesk_agents**: List helpdesk staff (agents)
- **list_kb_articles**: List knowledgebase articles
- **list_user_organizations**: List user organizations
- **list_helpdesk_tickets**: Supports filtering by status and department.

List helpdesk tickets
- **list_helpdesk_users**: List end-users
- **list_configured_webhooks**: List active webhooks
- **update_ticket_properties**: Modify an existing ticket


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deskpro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all helpdesk tickets with status 'awaiting_agent'."

**🤖 AI Agent:**
> I've retrieved 3 tickets awaiting attention. Highlights include 'Server Downtime' (Priority: High) and 'Billing Inquiry'. Would you like the message transcript for the high-priority case?

---

**👤 You:**
> "Show me the full history for ticket ID '123'."

**🤖 AI Agent:**
> Fetching transcript... Ticket 123 details a recurring login failure reported by @user. Agent Sarah provided troubleshooting steps 2 hours ago. The status is currently 'awaiting_user'. Shall I draft a follow-up?

---

**👤 You:**
> "Find articles in the knowledgebase about 'setup guide'."

**🤖 AI Agent:**
> Searching help center... I found 2 relevant articles: 'Quick Start Guide' (ID: 789) and 'Advanced Setup'. Would you like me to retrieve the full content for the Quick Start guide?


## ❓ FAQ

**Q: How do I find my Deskpro API Key?**
Log in as an Admin, navigate to **Apps & Integrations** > **API Keys**, and click **Add** to generate a new key for your instance.

**Q: Can the agent update ticket priorities?**
Yes! The `update_ticket_properties` tool allows the agent to modify status, urgency, and specific metadata of any support request.

**Q: Does it support reading internal articles?**
Absolutely. Use the `get_article_content` tool with an article ID to retrieve the full text and metadata for your help center content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deskpro](https://vinkius.com/mcp/deskpro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deskpro** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `deskpro` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deskpro** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deskpro": {
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
