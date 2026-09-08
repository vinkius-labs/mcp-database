# Workday Talent & Skills MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/workday-talent-skills)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Workday Talent & Skills Cloud as an MCP: people directory, direct reports, inbox tasks, worker skills (read + write) and organization headcount — official REST API v3 with OAuth 2.0 refresh-token auth.

## Description
The **talent side of Workday HCM** as a single MCP server — built on the official Workday REST API (v3) with the OAuth 2.0 refresh-token integration flow.

### What you can do
- **People directory** — search every person in the tenant (employees, contingent workers, alumni) by name, email or ID
- **Team views** — direct reports of any manager; headcount of any supervisory organization
- **Inbox tasks** — approvals and to-dos waiting on a worker (compensation changes, business process actions)
- **Skills Cloud** — read a worker's verified skill profile and **add skills** programmatically (Kotlin, Financial Analysis...)
- **Self check** — `workers/me` sanity check with your integration credentials

### Authentication (set up once, in your Workday tenant)
1. **Register API Client for Integrations** — creates the Client ID + Client Secret; grant the *Staffing/Talent* and *Worker* scopes your use case needs
2. **Manage Refresh Tokens for Integrations** — generate a non-expiring refresh token for the API Client, tied to an Integration System User (ISU) with a security group
3. Paste **Tenant URL** (e.g. `https://wd5-impl-services1.workday.com`), **Tenant Name**, Client ID, Client Secret and Refresh Token into this MCP's credentials

The MCP exchanges the refresh token at `POST /ccx/oauth2/{tenant}/token` for a Bearer access token (60-min expiry, auto-refreshed and cached) and calls `GET /ccx/api/v3/{tenant}/...` — official REST API v3 with `limit`/`offset` paging, WID and Reference IDs (`Employee_ID=21005`) and the `me` identifier.

### Who is this for?
HR ops teams, people analytics, talent management programs, internal tools and AI agents that automate Workday people/skills workflows.


## Available Tools (8)
- **get_my_profile**: Uses the REST API "me" identifier — the quickest sanity check that credentials work.

Get the Workday profile of the authenticated integration user (worker "me")
- **add_worker_skill**: Pass the skill name (e.g. "Kotlin") and optionally proficiency level (1-5 where applicable) and source note. The tenant must have Skills Cloud and the API Client must include the Staffing write scope for this to succeed.

Add a skill to a worker's profile (Skills Cloud write action)
- **search_people**: Returns descriptor, id (WID) and href for each person — use ids in other tools. Paging via page/limit (API max 100).

Search the Workday people directory (all persons, not just active workers)
- **get_inbox_tasks**: g. compensation change approvals, to-dos), each with id, descriptor and task type. Use "me" for the integration user or any worker id with proper scope.

List Workday inbox tasks for a worker (approvals, to-dos, action items)
- **get_worker_skills**: Requires a tenant with Skills Cloud enabled.

Get the Skills Cloud profile of a worker (verified skills, ratings, sources)
- **get_worker_direct_reports**: Each entry: descriptor, id, business title. For manager self-service and org reviews.

List the direct reports of a worker (their team as manager)
- **list_organizations**: Use ids to drill into an org's workers via get_org_workers.

Browse Workday organizations: companies, cost centers, supervisory orgs, regions
- **get_org_workers**: For headcount snapshots and org charts.

List the workers inside a supervisory organization (the org's headcount)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Workday Talent & Skills** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check my Workday credentials and show my profile"

**🤖 AI Agent:**
> 🏢 **Workday credentials OK**

Token exchanged successfully (60-min Bearer cached).

**Your profile (workers/me):**
- Name: Integration System User → delegated worker
- Business title: HR Integration Agent
- Organization: People Operations

Everything wired correctly. Want your inbox tasks or direct reports next?

---

**👤 You:**
> "What skills does employee 21005 have and add 'Prompt Engineering' to their profile"

**🤖 AI Agent:**
> 🧠 **Employee_ID=21005 — Skills Cloud**

Current skills (12): Python, SQL, Data Visualization, Stakeholder Management...

✅ Added **Prompt Engineering** — will appear as self-reported pending any verification policy your tenant enforces.

---

**👤 You:**
> "Who reports to employee 21005 and what approvals are pending for them?"

**🤖 AI Agent:**
> 👥 **Employee_ID=21005 — team & inbox**

Direct reports (7): including 2 Data Analysts and 1 Senior Engineer.

Inbox tasks (4 pending):
- Job Change approval — Compensation Review (due Friday)
- 2× Time Off approvals
- 1 To-Do: Complete annual review questionnaire

Want me to check the org's total headcount too?


## ❓ FAQ

**Q: How do I get the credentials this MCP needs?**
In your Workday tenant (admin role): 1) 'Register API Client for Integrations' → Client ID + Secret, granting Staffing/Talent scopes; 2) 'Manage Refresh Tokens for Integrations' → generate a refresh token for an Integration System User. Refresh tokens do not expire; the MCP converts them to 60-minute Bearer tokens automatically.

**Q: How is this different from the existing Workday MCP?**
The published Workday MCP covers workers, payroll, time off and supervisory orgs. This one is the talent angle: the people directory (all persons), direct reports, inbox tasks, Skills Cloud (read + write) and cross-type organizations — no overlapping tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/workday-talent-skills](https://vinkius.com/ai-agent-connect/workday-talent-skills)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Workday Talent & Skills** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `workday-talent-skills` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Workday Talent & Skills** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "workday-talent-skills": {
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
