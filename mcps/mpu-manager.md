# MPU-Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mpu-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Organize your media production workflow with asset tracking, schedule coordination, and crew management for broadcast teams.

## Description
Connect your **MPU-Manager** account to any AI agent and take full control of your medical-psychological assessment (MPU) orchestration and automated case management through natural conversation.

### What you can do

- **Client Case Orchestration** â€” List and manage your entire database of client files programmatically, retrieving detailed case metadata and legal statuses
- **Appointment & Schedule Intelligence** â€” Programmatically query and monitor assessment appointments to maintain a perfectly coordinated audit trail for your clinic
- **Assessment Architecture Monitoring** â€” Access real-time status updates for ongoing MPU cases and track document submission progress directly through your agent
- **Metadata Management** â€” Programmatically retrieve client identifiers and case history to maintain a perfectly coordinated digital archive
- **Operational Monitoring** â€” Verify account-level API connectivity and monitor case management volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your MPU-Manager dashboard (Settings > API)
3. Start orchestrating your case management from Claude, Cursor, or any MCP client

No more manual checking of paper files or missing critical assessment deadlines. Your AI acts as your dedicated case coordinator and clinic architect.

### Who is this for?

- **Clinic Managers** â€” instantly retrieve case summaries and monitor appointment volume using natural language commands
- **Legal Consultants** â€” verify individual client metadata and track assessment history without leaving your creative workspace
- **Developers** â€” integrate high-speed MPU-Manager case data into custom internal tools through simple AI queries


## Available Tools
- **check_mpumanager_status**: Verify MPU Manager API connectivity
- **create_appointment**: Schedule an appointment
- **create_case**: Create a new case
- **get_appointment**: Get appointment details
- **get_case**: Get case details
- **get_client**: Get client details
- **list_appointments**: List all appointments
- **list_cases**: List all cases
- **list_clients**: List all clients
- **list_reports**: List case reports


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MPU-Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all active cases in my account."

**🤖 AI Agent:**
> You have 15 active cases. 3 are high-priority with upcoming appointments this week. The most recent is Case #4821 (Maria Santos). Would you like to see details or appointments?

---

**👤 You:**
> "Schedule an appointment for case #4821 next Monday at 10am."

**🤖 AI Agent:**
> Appointment scheduled for Case #4821, Monday May 5 at 10:00am at your default office location. Confirmation sent. Would you like to add notes?

---

**👤 You:**
> "List all clients registered in my account."

**🤖 AI Agent:**
> You have 42 registered clients. The most recent is João Oliveira (added 3 days ago, 2 active cases). Would you like to see details or create a new case?


## ❓ FAQ

**Q: How do I create a new case via AI?**
Use the `create_case` tool with a client ID and description. The case is opened immediately in your MPU Manager account.

**Q: Can I schedule appointments from my agent?**
Yes. Use `create_appointment` with case ID, date (ISO 8601), and location to schedule a new appointment instantly.

**Q: How do I view reports for a specific case?**
Use `list_reports` with the case ID to retrieve all generated reports including type, date, and current status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mpu-manager](https://vinkius.com/mcp/mpu-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MPU-Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mpu-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MPU-Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mpu-manager": {
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
