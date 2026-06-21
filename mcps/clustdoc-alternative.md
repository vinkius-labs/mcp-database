# Clustdoc MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clustdoc-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Collect client documents, track submission progress, and streamline onboarding with organized intake workflows.

## Description
Connect your **Clustdoc** account to any AI agent and take full control of your professional client onboarding and automated document collection workflows through natural conversation.

### What you can do

- **Application Orchestration** — List and manage all active client applications programmatically, including monitoring completion percentages and real-time status changes
- **Document Architecture** — Organize and track the collection of critical business documents (KYC, contracts, IDs) by initializing high-fidelity application folders directly from your agent
- **Workflow Intelligence** — Access your directory of onboarding processes (templates) to ensure every new client follows the perfect perfectly coordinated legal and operational path
- **Team Coordination** — Retrieve directories of organization users and monitor team activities to oversee high-volume onboarding pipelines efficiently
- **Operational Monitoring** — Check active webhooks and retrieve specific application metadata directly through your agent for instant auditing and reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** (Bearer) from your Clustdoc dashboard (Settings > API)
3. Start managing your client pipeline from Claude, Cursor, or any MCP client

No more manual following up on missing files or digging through student/client folders in the portal. Your AI acts as your dedicated onboarding specialist and document coordinator.

### Who is this for?

- **Account Managers & Legal Teams** — instantly retrieve application summaries and check document completion using natural language commands
- **Operations Specialists** — automate the creation of new client files and track progress without leaving your communication tools
- **Real Estate & HR Leads** — monitor incoming tenant or employee applications and retrieve finalized PDFs through simple AI queries


## Available Tools
- **create_application**: Pass data as a JSON string.

Create a new application
- **get_application_details**: Get specific application details
- **list_applications**: List all client applications
- **list_workflows**: List all onboarding workflow processes
- **list_team_members**: List all team members
- **list_webhooks**: List all configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clustdoc** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active client applications in Clustdoc."

**🤖 AI Agent:**
> I've retrieved your applications. You currently have 5 active submissions, including 'Alice Brown' (75% complete) and 'TechCorp KYC'. Which one would you like the full step-by-step progress for?

---

**👤 You:**
> "Create a new onboarding file for 'John Doe' using the 'KYC' process."

**🤖 AI Agent:**
> Application created! John Doe has been successfully initialized in your Clustdoc workspace using the KYC template. You can share his personal portal link to begin document collection: [portal_url].

---

**👤 You:**
> "Show me the list of all onboarding team members."

**🤖 AI Agent:**
> I've retrieved your team directory. You currently have 3 active members overseeing applications: @admin, @sarah, and @mike. Shall I check who is assigned to your most recent submission?


## ❓ FAQ

**Q: How do I find my Clustdoc API Token?**
Log in to your account, navigate to **Settings** > **API**, and generate or copy your unique Bearer Token.

**Q: Can I start a specific onboarding process via AI?**
Yes! The `create_application` tool allows you to specify a `process_id` to trigger the exact workflow template you need.

**Q: How do I check document completion status?**
Use the `get_application_details` tool with an application ID to retrieve high-fidelity metadata including the current step and completion progress.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clustdoc-alternative](https://vinkius.com/mcp/clustdoc-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clustdoc** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `clustdoc-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clustdoc** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clustdoc-alternative": {
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
