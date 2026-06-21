# CloudCard ID Photos MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudcard-id-photos)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage ID photo submissions, approvals, and cardholder data via CloudCard directly from your AI agent.

## Description
Empower your AI agent with access to the **CloudCard** (RemotePhoto) platform to automate your ID card production and photo approval workflows.

### What you can do

- **Photo Approval Workflow**. List submitted photos and approve or deny them with specific reason codes directly through natural language.
- **Cardholder Management**. Register new people (students/employees) and retrieve detailed profile and submission history.
- **Submission Standards**. Access organization-level photo requirements and dimensions to ensure high-quality ID production.
- **Operational Oversight**. Monitor event webhooks, check API health status, and retrieve distribution office locations.

### How it works

1. Subscribe to this server
2. Enter your CloudCard API Token (X-Auth-Token)
3. Start managing your ID production from Claude, Cursor, or any MCP client

### Who is this for?

- **University Registrar Offices**. Quickly approve student ID photos and check submission statuses via natural conversation.
- **Corporate HR Teams**. Manage employee photo uploads and card production without leaving your workspace.
- **Security & Access Control**. Automate cardholder registration and monitor photo requirements using natural language commands.


## Available Tools (12)
- **approve_id_photo**: Approve a submitted photo
- **check_api_health**: Verify CloudCard API connectivity
- **register_new_cardholder**: Requires email and first/last name.

Add a new person to CloudCard
- **deny_id_photo**: Requires a reason code or message for the cardholder.

Deny a submitted photo
- **get_authenticated_profile**: Get current API user info
- **get_organization_settings**: Get organization metadata
- **get_cardholder_details**: Get details for a specific person
- **list_card_offices**: List distribution locations
- **list_cardholders**: List all cardholders (people)
- **list_submitted_photos**: Supports filtering by status.

List all photo submissions
- **list_photo_requirements**: g., format, size, background).

Get submission requirements
- **list_configured_webhooks**: List active event webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CloudCard ID Photos** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all pending photo submissions in CloudCard."

**🤖 AI Agent:**
> I've found 12 pending photo submissions. Notable ones include John Doe (ID: 123) and Alice Smith. Would you like to review their photos?

---

**👤 You:**
> "Deny photo ID '789' because the background is not plain white."

**🤖 AI Agent:**
> Done! I've denied photo '789' with the reason: 'Background is not plain white'. The cardholder will be notified.

---

**👤 You:**
> "Show me the details for cardholder 'john@example.com'."

**🤖 AI Agent:**
> I've retrieved John Doe's profile. He has one approved photo and his physical ID card was picked up at the Main Office on April 10th.


## ❓ FAQ

**Q: How do I get a CloudCard API Token?**
Log in to your [**CloudCard Admin**](https://app.cloudcard.us/) portal, go to your Profile or Settings, and generate an API Token (X-Auth-Token).

**Q: Can the agent auto-approve photos?**
Yes, using the `approve_id_photo` tool, the agent can approve any pending photo submission once verified through conversation.

**Q: Is student ID management supported?**
Absolutely. CloudCard is widely used in higher education, and this server supports registering students and managing their photo submissions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudcard-id-photos](https://vinkius.com/mcp/cloudcard-id-photos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CloudCard ID Photos** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cloudcard-id-photos` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CloudCard ID Photos** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cloudcard-id-photos": {
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
