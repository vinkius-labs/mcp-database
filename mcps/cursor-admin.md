# Cursor Admin MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cursor-admin)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your Cursor team — list members, audit logs, usage data, spending, repo blocklists, and team settings via the Cursor Admin API from any AI agent.

## Description
Connect your **Cursor Admin** API key to any AI agent and manage your team through natural conversation.

### What you can do

- **Team Member Management** — List all team members with their roles, emails, and removal status. Remove members by email or user ID when needed
- **Audit Logs** — Retrieve administrative audit events filtered by time range, event types, search text, or specific users. Track team_settings changes, member_management actions, and billing events
- **Daily Usage Analytics** — Pull per-user daily usage metrics including lines added/deleted, tab completions, apply/accept/reject counts, and composer/chat/agent request counts
- **Spending Management** — View team spending with per-member breakdowns (spendCents, fastPremiumRequests, monthlyLimitDollars). Set or remove individual spend limits for budget control
- **Usage Events** — Get detailed usage events with model names, request kinds, token usage, and charged amounts for cost attribution
- **Repository Blocklists** — Manage which repositories are blocked from AI indexing. View current blocklists with URL and pattern rules, and add or update entries
- **Team Settings** — Retrieve and update team configuration settings
- **Team Info** — Get team metadata including name, member count, and plan details

### How it works

1. Subscribe to this server
2. Enter your Cursor Admin API key (create one at Cursor Dashboard → API Keys, requires admin:* scope)
3. Start managing your team from Claude, Cursor, or any MCP-compatible client

Your AI acts as a team administration gateway — monitor usage, control spending, review audit logs, and manage members without writing a single line of code.

### Who is this for?

- **Team Administrators** — manage members, review audit logs, and enforce spending policies through natural language
- **Engineering Managers** — track team usage patterns, monitor AI adoption, and identify power users or potential misuse
- **Finance Teams** — pull spending data for billing cycles, set per-user spend limits, and monitor costs
- **Security Teams** — review audit logs for suspicious activity, manage repo blocklists, and ensure compliance with data access policies


## Available Tools (12)
- **get_audit_logs**: Supports pagination via page and pageSize. Event types include team_settings, member_management, billing, and other administrative actions. Returns events array plus pagination metadata.

Retrieve audit logs for the team with optional filters
- **get_daily_usage_data**: startDate and endDate are epoch milliseconds. Supports optional pagination.

Retrieve per-user daily usage metrics for a date range
- **get_repo_blocklists**: Repo blocklists prevent AI from indexing or accessing specified repositories.

Retrieve the repository blocklist configuration
- **get_spending_data**: Supports search, sorting, and pagination. Use this for billing cycles and budget monitoring.

Retrieve team spending data with per-member breakdowns
- **get_team_info**: [INFERENCE] The endpoint path /teams/info is inferred from REST conventions; no explicit documentation exists for this endpoint.

Retrieve team metadata and overview information
- **get_team_settings**: [INFERENCE] The endpoint path /teams/settings is inferred from REST conventions and the fact that team_settings appears as an audit event type in the Admin API documentation.

Retrieve the current team settings
- **get_usage_events**: Filter by date range, user, service account, and hosting type. Supports pagination. Useful for detailed usage analysis and cost attribution.

Retrieve filtered usage events for the team
- **list_team_members**: Use this to see who is on the team and their current roles.

List all team members in the organization
- **remove_team_member**: This is a destructive operation — the member will lose access to the team. Provide either email or user_id to identify the member. Returns success status and the affected user ID.

Remove a team member from the organization
- **set_user_spend_limit**: Pass null for spend_limit_dollars to remove an existing spend limit. Returns an outcome and message indicating success or failure. Note: This endpoint has a higher rate limit of 250 req/min.

Set or remove the spend limit for a specific team member
- **update_team_settings**: Only the fields included in settings_json will be modified. [INFERENCE] The endpoint path /teams/settings with POST is inferred from REST conventions.

Update team settings with partial configuration
- **upsert_repo_blocklists**: Pass a JSON array of repos, each with a url and a patterns array. Existing entries with matching URLs are updated; new entries are created. [INFERENCE] The exact response shape is inferred from the REST pattern.

Add or update repository blocklist entries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cursor Admin** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all team members and show their roles."

**🤖 AI Agent:**
> Found 8 team members:
- **Alice Chen** (admin) — alice@example.com
- **Bob Smith** (member) — bob@example.com
- **Carol Jones** (member) — carol@example.com
- **David Wilson** (admin) — david@example.com
- **Eve Brown** (member) — eve@example.com
- **Frank Garcia** (member) — frank@example.com
- **Grace Lee** (member) — grace@example.com
- **Henry Taylor** (member, removed) — henry@example.com

7 active members and 1 removed. 2 admins and 5 regular members. Would you like to see usage data or spending details for any of these members?

---

**👤 You:**
> "Get spending data for the current billing cycle."

**🤖 AI Agent:**
> Here's the team spending summary for the current billing cycle:

- **Alice Chen** — $45.20 (fast premium requests: 23)
- **Bob Smith** — $12.80 (fast premium requests: 6)
- **Carol Jones** — $87.50 (fast premium requests: 41) ⚠️ exceeds monthly limit of $50
- **David Wilson** — $33.10 (fast premium requests: 15)
- **Eve Brown** — $5.40 (fast premium requests: 2)

**Total team spend: $184.00**

Carol Jones has exceeded her monthly spend limit of $50. Would you like to adjust her spend limit or review her usage events for more details?

---

**👤 You:**
> "Check the audit logs for security events in the last 7 days."

**🤖 AI Agent:**
> Retrieved 14 audit events from the last 7 days. Here are the notable security-related events:

1. **member_management** — Henry Taylor was removed from the team by David Wilson (2026-07-08)
2. **team_settings** — Repository blocklist updated by Alice Chen: added https://github.com/org/secret-repo with patterns [*.env, secrets/*] (2026-07-07)
3. **team_settings** — Spend limit set for Carol Jones: $50/month by David Wilson (2026-07-06)
4. **member_management** — Grace Lee role changed from member to admin by Alice Chen (2026-07-05)
5. **billing** — Monthly billing cycle started (2026-07-04)

No suspicious or unauthorized activity detected. All changes were performed by known admin users. Would you like to filter by a specific event type or user for a deeper review?


## ❓ FAQ

**Q: How do I get my Cursor Admin API key?**
Go to the Cursor Dashboard → Settings → API Keys to create an admin API key. The key starts with `crsr_` and must have the `admin:*` scope to access the Admin API. Copy the key and paste it into the API key field in the setup wizard. The key is sent as Basic Auth credentials (API key as the username, empty password) in every request to `https://api.cursor.com`.

**Q: What API scope is required?**
The Admin API requires the `admin:*` scope on your API key. This scope grants access to team management, audit logs, usage data, spending controls, and team settings. Without the admin scope, API calls will return 401 Unauthorized. Generate your key from an admin account in the Cursor Dashboard.

**Q: What are the rate limits?**
The Admin API has a rate limit of 20 requests per minute for most endpoints. The `set_user_spend_limit` endpoint has a higher limit of 250 requests per minute. If you exceed the rate limit, the API returns a 429 status code. The engine handles retries transparently where appropriate, but for bulk operations, consider spacing your requests.

**Q: Can I manage team spending and set spend limits?**
Yes. Use `get_spending_data` to view per-member spending breakdowns including spendCents, overallSpendCents, fastPremiumRequests, and monthlyLimitDollars. Use `set_user_spend_limit` to set a monthly spend limit in dollars for any team member, or pass null to remove an existing limit. The spend limit endpoint has a higher rate limit of 250 requests per minute.

**Q: Are audit logs available for security review?**
Yes. Use `get_audit_logs` to retrieve administrative audit events. You can filter by time range (startTime/endTime), event types (e.g. team_settings, member_management, billing), search text, and specific users. The response includes event types, timestamps, and descriptions of administrative actions. This is valuable for security reviews and compliance audits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cursor-admin](https://vinkius.com/mcp/cursor-admin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cursor Admin** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cursor-admin` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cursor Admin** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cursor-admin": {
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
