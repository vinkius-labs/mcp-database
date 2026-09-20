# 1Password SaaS Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/1password-saas-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Govern your 1Password organization for AI agents: catalog SaaS apps, inspect people and teams, read the audit log, and run automation workflows.

## Description
Connect your **1Password organization** to any AI agent through the 1Password SaaS Manager API. This server governs the organization itself — the SaaS catalog, the people and teams that use it, the audit trail, and the automation workflows — so an agent can reason about access and act on the controls your team has set up.

### What you can do

- **SaaS Catalog** — List the applications your organization tracks and inspect any one of them in detail
- **People & Teams** — See who is in the organization and how the teams are structured
- **Audit Trail** — Read the audit log for who did what and when, narrowed by time window
- **Automation** — Discover the defined workflows, inspect a specific run, and fire a signal to advance or gate a step

### How it works

1. Create API client credentials for the SaaS Manager in your 1Password organization (choose the US or EU region)
2. Paste the Client ID and Client Secret into this server's credential fields, and set the base URL to match your region
3. Ask your agent to reason about the catalog, the people, the audit trail, or the automations — the server signs short-lived tokens on its own

### Who is this for?

- **Security & Compliance Teams** — keep the SaaS inventory current, surface audit events, and drive the review workflows that gate new access
- **Identity Administrators** — check team structure and membership before making access changes


## Available Tools (8)
- **fire_workflow_signal**: This is a state-changing operation: only fire it when the user explicitly asks to advance or unblock a run. The activity ID and available signal names come from get_workflow_run; some activities run multiple iterations, in which case iterationId selects one.

Fire a signal on an activity of a 1Password workflow run
- **list_teams**: Use when the user asks about team structure, who belongs where, or before reasoning about group-level access. For the team hierarchy, the same endpoint family returns nesting — treat each entry as one team and group by parent fields present in the data.

List the teams in the 1Password organization
- **list_workflows**: Use when the user wants to see available automations or find one by name before looking at its runs. The workflow ID from this list is the input for get_workflow_run and fire_workflow_signal.

List the automation workflows in 1Password SaaS Manager
- **get_application**: Use after locating an app with list_applications, or when the user names a specific app to inspect. The application ID comes from list results.

Read one SaaS application from the 1Password catalog
- **get_workflow_run**: Use when a workflow appears stuck or the user asks what happened in one run. The workflow ID and run ID come from list_workflows and the organization's run history.

Inspect one run of a 1Password automation workflow
- **list_applications**: Use when the user asks what SaaS apps the company uses, which are visible or active, or before picking an app to inspect. Page through results by passing the cursor from the previous response as after; cap pages with limit.

List the SaaS applications managed in the 1Password organization catalog
- **list_audit_events**: Use for compliance questions: who did what, sign-in anomalies, permission changes. Narrow the window with since/until (ISO dates) to keep pages small; page with after.

Read the 1Password audit log
- **list_people**: Use for headcount questions, finding a person, or checking membership status. Pass the cursor from a previous response as after to continue; cap with limit.

List people (users) in the 1Password organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **1Password SaaS Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which SaaS applications are active in our organization right now?"

**🤖 AI Agent:**
> I listed the tracked applications and filtered to the active ones. You have 14 active SaaS apps: Slack, Confluence, Salesforce, Okta, Datadog, Jira, Linear, Notion, GitHub, AWS, GCP, Zendesk, Intercom and Retool. Want the detail on any of these?

---

**👤 You:**
> "Show me audit log events from the last 48 hours where admin permissions changed."

**🤖 AI Agent:**
> I read the audit log for the past 48 hours. Three admin-permission events stand out: 2) a service account was granted admin on the Slack app, 4) two people left the 'Security' team, and 1) a new app was added to the catalog by an admin. The service-account grant is the one to review first — do you want me to pull that event in full?

---

**👤 You:**
> "Our onboarding workflow is stuck on step 3. Check that run and tell me what it's waiting for."

**🤖 AI Agent:**
> I pulled the workflow run. Step 3, the access-grant activity, is waiting on a 'continue' signal — it's gated on a manual confirmation that a manager approves the new person's team access. Nothing has advanced in the last 2 days. Want me to fire the 'continue' signal to unblock it?


## ❓ FAQ

**Q: Which parts of 1Password does this manage?**
The SaaS Manager organization surface: the SaaS application catalog, people, teams, the audit log, and automation workflows. It does not read or manage personal vault items or individual secrets — those are out of scope for this server.

**Q: How does authentication work?**
Machine-to-machine OAuth 2.0 client-credentials. The server exchanges your Client ID and Client Secret for a short-lived bearer token and signs its own requests — no human login, no user session. The base URL selects the region: app.trelica.com (US) or eu.trelica.com (EU).

**Q: Can it change the organization, or only read it?**
Mostly read. The read tools cover the catalog, people, teams, audit log, workflow definitions, and runs. The one state-changing tool is fire_workflow_signal, which advances or gates a step of an automation run — use it only when explicitly asked.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/1password-saas-manager](https://vinkius.com/en/ai-agent-connect/1password-saas-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **1Password SaaS Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `1password-saas-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **1Password SaaS Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "1password-saas-manager": {
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
