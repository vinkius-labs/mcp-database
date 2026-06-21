# Sentry MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sentry-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Monitor errors and application health via Sentry — query issues, inspect events, audit releases and check alert rules directly from any AI agent.

## Description
Connect your **Sentry** account to any AI agent and gain real-time observability over your application errors through natural conversation.

### What you can do

- **Organization & Project Discovery** — List all Sentry organizations, teams and projects with full configuration details
- **Issue Management** — Browse, inspect and update error issues. Change status (resolve, mute, delete) or assign issues to team members
- **Event Inspection** — Retrieve raw error events with complete stacktraces, breadcrumbs, HTTP context and user data to debug root causes
- **Release Tracking** — List all application releases, view deployment metadata and correlate issues to specific versions
- **Alert Rules Auditing** — Review configured alert rules (Slack, email, PagerDuty triggers) to understand your team's notification pipeline
- **Tag Analysis** — View all event tags (environment, release, transaction) for filtering and grouping errors

### How it works

1. Subscribe to this server
2. Enter your Sentry Internal Integration Token
3. Start monitoring your apps from Claude, Cursor, or any MCP-compatible client

Stop context-switching to the Sentry dashboard every time an alert fires. Your AI acts as a dedicated on-call engineer.

### Who is this for?

- **On-Call Engineers** — instantly triage new errors, view stacktraces and check if issues are resolved without opening Sentry
- **Engineering Managers** — audit alert rules, monitor release health and review open issue counts across all projects
- **Developers** — search for specific errors, inspect event breadcrumbs and verify which release introduced a regression


## Available Tools
- **list_alert_rules**: Each rule defines conditions (e.g. "issue created more than X times in 5 minutes"), actions (Slack, email, PagerDuty) and target channels/users.

List alert rules in a Sentry organization
- **get_auth_info**: Use this to verify your token is working correctly.

Get authentication info for the current Sentry token
- **list_events**: Events contain the error message, stacktrace snippets, platform, environment and timestamps. Useful for auditing what errors have been firing recently.

List recent events for a Sentry project
- **get_event**: Use the event ID returned from list_events.

Get full details for a specific Sentry event
- **get_issue**: Use the numeric issue ID.

Get full details for a Sentry issue
- **get_project**: Provide both the organization slug and project slug.

Get details for a specific Sentry project
- **get_release**: Use the organization slug and the exact release version string.

Get details for a specific Sentry release
- **list_issues**: Can list issues organization-wide or scoped to a specific project. Use the query parameter to filter by status, priority, first release, timestamp or text search. Example query: "is:unresolved priority:50".

List issues in a Sentry organization or project
- **list_organizations**: Each organization has a unique slug, name, access permissions and team/member information. Use the organization slug for subsequent API calls.

List all Sentry organizations
- **list_projects**: Each project tracks errors for a specific application or service and has settings for alerts, environments and team ownership. Provide the organization slug.

List projects in a Sentry organization
- **list_releases**: Use to track which versions have been deployed and correlate issues to specific releases.

List releases for a Sentry organization or project
- **search_issues**: Uses the Sentry query syntax. Can be scoped to an entire organization or a specific project. Returns matching issues with count, priority, status and first/last seen timestamps.

Search Sentry issues by text
- **list_tags**: ) used to categorize events. Tags are essential for filtering and grouping issues in Sentry.

List tags for a Sentry organization or project
- **list_teams**: Each team has members, projects and access control settings. Provide the organization slug to list its teams.

List teams in a Sentry organization
- **update_issue**: Can also add/remove tags. Provide the numeric issue ID and the desired status.

Update a Sentry issue status or assign it


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sentry** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all unresolved issues in my backend-api project."

**🤖 AI Agent:**
> I've scanned your backend-api project and found 4 unresolved issues. The most critical is a `ZeroDivisionError` in payment processing (127 events in the last 24h). Would you like the full stacktrace?

---

**👤 You:**
> "Which releases have been deployed for my organization in the last month?"

**🤖 AI Agent:**
> I've retrieved 6 releases for your organization. The most recent is `v2.14.3` deployed 2 days ago to the production environment. The oldest in this window is `v2.12.0` from 28 days ago. Would you like event counts per release?

---

**👤 You:**
> "What alert rules are currently configured for the mobile-app team?"

**🤖 AI Agent:**
> Your mobile-app project has 3 active alert rules: 1) Notify #eng-mobile on Slack when a new issue is created, 2) Send email to oncall@company.com when issue count exceeds 100 in 5 minutes, 3) Create PagerDuty incident for errors with priority 50. Would you like the full configuration details for any rule?


## ❓ FAQ

**Q: How do I create a Sentry Internal Integration Token?**
Go to your [**Sentry Organization Settings**](https://sentry.io/settings/), select **API Keys** > **Create New Integration**. Name it (e.g. 'Vinkius MCP'), select the scopes you need (recommended: `org:read`, `project:read`, `event:read`, `team:read`, `release:read`), and click **Save**. Copy the token immediately — it starts with `sntrys_` and won't be shown again.

**Q: Can I resolve or mute an issue directly from the agent?**
Yes! Use the `update_issue` action with the issue's numeric ID and set `status` to `resolved` (marks it fixed), `muted` (hides it from the inbox) or `deleted` (removes it permanently). You can also reassign issues using the `assigned_to` parameter.

**Q: What Sentry query syntax does the search support?**
Sentry uses its own query syntax. Common filters include: `is:unresolved` (open issues), `is:resolved` (fixed issues), `priority:[1-50]` (priority levels), `first_release:1.2.3` (issues introduced in a specific release), `user.email:example@co.com` (errors affecting a specific user). You can combine filters: `is:unresolved priority:50`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sentry-alternative](https://vinkius.com/mcp/sentry-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sentry** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sentry-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sentry** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sentry-alternative": {
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
