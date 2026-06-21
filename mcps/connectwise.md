# ConnectWise MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/connectwise)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Equip your AI to seamlessly manage ConnectWise PSA tickets, clients, and technical documentation via text.

## Description
Empower your conversational AI with deep integration into **ConnectWise Manage (PSA)**. Enhance technical support operations by enabling your agent to triage issues, update existing service tickets, and retrieve critical client environment data without leaving your conversational interface.

### What you can do

- **Ticketing Operations** — Rapidly inspect queue statuses, assign incoming tickets, or update internal notes naturally.
- **Asset & Configuration Retrieval** — Look up devices, configurations, and agreements associated with a specific managed client.
- **Billing & Time Entries** — Log billable technical time or adjust status workflows directly through the chat.

### How it works

1. Attach the ConnectWise tool to your preferred MCP interface.
2. Supply your designated Company ID, Public Key, and Private Key for secure authentication.
3. Chat seamlessly with your agent to govern your helpdesk and IT services.

### Who is this for?

- **Level 1/2 Support Technicians** — Quickly triage, update notes, and close straightforward tickets without bogging down in complex UI menus.
- **Service Delivery Managers** — Audit ticket lifecycles, check SLA compliance, and monitor board queues efficiently.
- **MSP Owners** — Pull immediate reports on client profitability or check current active incidents directly from a mobile chat.


## Available Tools (9)
- **create_ticket**: Create a new service ticket in ConnectWise Manage
- **get_company**: Returns name, contact info, territory, and status.

Retrieve detailed information about a specific company
- **get_ticket**: Returns summary, priority, status, assigned member, and notes.

Retrieve detailed information about a specific service ticket
- **list_sales_activities**: Retrieve a list of sales and service activities
- **list_companies**: Use to discover company identifiers for ticket creation.

Retrieve a list of companies/clients in ConnectWise
- **list_contacts**: Use to find external contact details.

Retrieve a list of individual contacts within companies
- **list_members**: Retrieve a list of internal staff members
- **list_service_tickets**: Supports pagination via pageSize.

Retrieve a list of service tickets from ConnectWise Manage
- **search_tickets_by_summary**: Useful for finding tickets by keyword.

Find service tickets matching a keyword in the summary


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ConnectWise** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the top 3 open critical tickets currently on the 'Helpdesk' board."

**🤖 AI Agent:**
> Certainly. Finding tickets on the 'Helpdesk' board filtered by 'Critical' status and 'Open' state: 1) Ticket #14052: Core Switch Failure (Client: Initech), 2) Ticket #14057: Ransomware containment active (Client: Massive Dynamic), 3) Ticket #14099: CEO Email offline (Client: Globex). Would you like to view the internal notes for #14052?

---

**👤 You:**
> "Enter a time entry of 1.5 hours for ticket #13988 with the notes 'Reconfigured firewall rules to establish stable VPN tunnels.' and mark the ticket as closed."

**🤖 AI Agent:**
> Time entry created successfully. Logged 1.5 hours on Ticket #13988 associated with your active user credentials. Internal notes have been strictly appended as requested, and the ticket status has been securely transitioned from 'In Progress' to 'Closed'. Great work.

---

**👤 You:**
> "Retrieve the billing details and active agreements for the client 'Globex Corporation' to prepare for an audit."

**🤖 AI Agent:**
> Retrieving financial matrices reliably...
**Client Record (`get_company_agreements`)**:
- Target: `Globex Corporation`
- Active Agreements: 2 (Managed IT Services, Cloud Backup SLA).
- Overdue Invoices: None detected structurally.
Audit preparation data retrieved successfully and accurately.


## ❓ FAQ

**Q: How do I securely obtain my ConnectWise API Keys and Company ID?**
Log into your ConnectWise Manage instance. Note your 'Company ID' prominently displayed on the login screen. Then navigate securely via the internal system module down under 'System' > 'Members', find the specialized sub-tab marked 'API Members'. Create a new specific role API member for this AI, and within its configuration, strictly establish a new API Key generation. This will output a matched pair containing your 'Public Key' and your strictly secured 'Private Key'. Securely provide all three specific parameters below.

**Q: Will the agent close tickets automatically, or must I specifically instruct it to change the status?**
The AI remains tightly compliant to your direct prompts. It will not spontaneously close unprompted tickets or mutate parameters heavily without instruction. You must expressly request 'Change ticket X status to Closed' ensuring governance, compliance, and accurate logging remains strictly under your control at all times during interactive use.

**Q: Can I query client configurations or passwords with this active integration?**
Configurational details such as device types and basic network data models are queryable if permissions via API permit, but sensitive field extraction like retrieving unencrypted passwords directly inside the dialog typically stays strictly masked or gated, abiding exclusively by your ConnectWise native security role allowances configured previously inside the specific 'API Member' settings during your setup.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/connectwise](https://vinkius.com/mcp/connectwise)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ConnectWise** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `connectwise` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ConnectWise** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "connectwise": {
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
