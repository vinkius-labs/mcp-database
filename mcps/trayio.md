# Tray.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/trayio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Equip your AI agent to orchestrate automations, track active workflows, and monitor data execution flows across Tray.io natively.

## Description
Connect your AI agent exclusively to your **Tray.io** (or Tray.ai) integration workflows. Bypass cumbersome cloud panels and directly manage automations, integrations, and solutions within a conversational interface. Allow your operations team or architects to audit workflows and supervise massive data transfer nodes organically, checking for health or broken loops in plain text.

### What you can do

- **Inventory Verification** — Audit all current integration solutions, mapping how data moves inside the entire architectural setup instantly
- **Workflow Discovery** — Instantly list and read metadata components or current triggers attributed to single active workflows
- **Live Monitoring** — Investigate the execution history logs on specific workflows to strictly certify which nodes succeeded or crashed during testing
- **Component Assessment** — Browse global lists of ready-to-use Connectors (like Salesforce, Stripe, Zendesk) directly out of your machine before mapping an integration strategy
- **Session Integrity** — Ping the core system to evaluate user identity tokens, boundaries, and regional connections to guarantee uptime

### How it works

1. Attach the application component to your generative environment
2. Provide your Tray Access Token and optional regional endpoint configuration directly on the portal slot
3. Engage the agent to audit operations or evaluate broken integration loops organically

### Who is this for?

- **Integration Architects** — Drill down into execution health metrics observing failures on complex CRM connections via conversation instead of traversing dashboards
- **Operations Leaders** — Swiftly assess which integrations or pipelines (Workflows) are publicly active mapping data inside the organization effortlessly
- **Support Teams** — Read the recent log failures (Executions) to troubleshoot bugs when client software instances fail to sync safely


## Available Tools
- **get_authenticated_user**: Retrieves details for the currently authenticated user
- **get_workflow_details**: Retrieves details for a specific Tray.io workflow
- **list_available_connectors**: g., Salesforce, Slack) can be integrated.

Lists all available service connectors in Tray.io
- **list_workflow_executions**: Lists recent execution history for a specific workflow
- **list_integration_solutions**: Lists all solutions (integration templates) in the account
- **list_workflows**: Lists all workflows in the Tray.io account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tray.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active workflows in my account right now."

**🤖 AI Agent:**
> I've pulled a total of 3 active workflows from your repository:
- Name: Salesforce Lead Sync, ID: wf-a1b2
- Name: Zendesk Ticket Router, ID: wf-c3d4
- Name: Stripe Financial Log, ID: wf-e5f6

---

**👤 You:**
> "Can you check the latest execution history for workflow wf-a1b2?"

**🤖 AI Agent:**
> Checking execution logs for wf-a1b2. The last 2 runs completed successfully with status: SUCCEEDED. The latest run took 4.2 seconds on 2026-10-05T14:22:11Z. No anomalous behavior detected locally.


## ❓ FAQ

**Q: Where do I find my primary Tray.io Access Token?**
Log in precisely through your Tray.io admin interface. Focus toward the user settings and click heavily on 'Profile' located usually top-right corner or bottom-left depending on your tier. Inside, shift directly to Personal Access Tokens to view the encoded array. Keep generated values incredibly safe as they orchestrate mass systems.

**Q: How important is defining the TRAY_REGION property?**
The API fundamentally varies endpoints based on your region (e.g., `us1`, `eu1`, `apac1`). If unassigned or blank, it legally defaults to `us1`. If your instance is physically nested anywhere else in global scope, you must insert your region, or your API logs will constantly fail resolving token access domains.

**Q: Should I use a User Token or a Master Token for the Tray MCP?**
You must use the Master Token. The Master Token acts as an administrative key allowing you to list authentications and orchestrate workflows across your organization's workspace, whereas a User Token is restricted.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/trayio](https://vinkius.com/mcp/trayio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tray.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `trayio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tray.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "trayio": {
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
