# PostHog MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/posthog-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage product analytics and feature flags via PostHog — query events, inspect cohorts, toggle flags and create annotations from any AI agent.

## Description
Connect your **PostHog** account to any AI agent and gain full control over your product analytics, feature flags and user cohorts through natural conversation.

### What you can do

- **User & Project Discovery** — Verify your account access and list all analytics projects
- **Feature Flag Management** — List, create, update and delete feature flags with rollout configuration
- **Cohort Inspection** — Review all behavioral cohorts and their filter definitions
- **Person Analytics** — Look up individual users by distinct ID, view their properties and activity timeline
- **Event Tracking** — Browse recent events, filter by event type and inspect event properties
- **Timeline Annotations** — Create and review annotations that correlate metric changes with deployments or launches

### How it works

1. Subscribe to this server
2. Enter your PostHog Personal API Key
3. Start managing your product analytics and feature flags from Claude, Cursor, or any MCP-compatible client

Stop switching between PostHog dashboards to check flag status or review event data. Your AI acts as a dedicated product analytics engineer.

### Who is this for?

- **Product Managers** — audit feature flag rollout percentages, review cohort definitions and create annotations for launches
- **Developers** — toggle feature flags, inspect event payloads and verify person properties without opening the PostHog UI
- **Data Analysts** — browse recent events, review person profiles and cohort membership for analysis


## Available Tools (13)
- **create_annotation**: Annotations appear on insights graphs and help correlate metric changes with deployments, launches or incidents. Requires the content text. Optionally set a date_marker (ISO 8601 date).

Create a new annotation in PostHog
- **create_feature_flag**: Requires the flag key (unique identifier). Optionally set the name, description, enabled status, rollout percentage and filters. The key must be unique across all flags in the project.

Create a new PostHog feature flag
- **delete_feature_flag**: All targeting conditions, release conditions and experiment data associated with the flag will be deleted. Provide the numeric flag ID. WARNING: this action is irreversible.

Delete a PostHog feature flag
- **get_feature_flag**: Provide the numeric flag ID from list_feature_flags.

Get details for a specific PostHog feature flag
- **get_person**: Provide the distinct_id used to identify the person.

Get details for a specific person in PostHog
- **get_user**: Returns user ID, email, name, organization membership and permissions. Use this to verify your API key is working and check your access level.

Get the current PostHog user details
- **list_annotations**: Annotations are markers on timeline graphs that highlight important events like deployments, feature launches or incidents. Returns annotation ID, content, date marker and whether it is pinned.

List annotations in PostHog
- **list_cohorts**: Each cohort is a dynamic group of users defined by event-based or property-based filters. Returns cohort ID, name, description, whether it is calculated or static.

List behavioral cohorts in PostHog
- **list_events**: Optionally filter by event name (e.g. "pageview", "signup", "purchase") and set a limit. Each event includes the event name, timestamp, person distinct ID and properties.

List events tracked in PostHog
- **list_feature_flags**: Each flag has a key, name, enabled status, rollout percentage, filters and release conditions. Returns flag ID, key, name, whether it is active, and the targeting configuration. Use this to audit feature flag coverage.

List all feature flags in PostHog
- **list_persons**: Each person has distinct IDs, properties, creation date and last event timestamp. Optionally set limit (default 20) and offset for pagination.

List persons (users) tracked in PostHog
- **list_projects**: Each project is an analytics workspace with its own events, persons, feature flags and cohorts. Returns project ID, name, organization and creation date.

List PostHog projects
- **update_feature_flag**: Provide the flag ID and any fields to change: name, description, enabled status. Only the fields you provide will be updated.

Update an existing PostHog feature flag


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PostHog** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all feature flags and which ones are enabled."

**🤖 AI Agent:**
> I found 8 feature flags. 5 are currently enabled: 'new-checkout' (80% rollout), 'dark-mode' (100%), 'ai-suggestions' (25%), 'beta-dashboard' (50%) and 'export-v2' (100%). 3 are disabled: 'legacy-search', 'old-onboarding' and 'deprecated-api'.

---

**👤 You:**
> "Create an annotation for today's deployment of version 3.2.0."

**🤖 AI Agent:**
> Done! I've created an annotation 'Deployed v3.2.0' pinned to today's date. It will appear on all relevant insights graphs so you can correlate any metric changes with this deployment.

---

**👤 You:**
> "Show me the profile of user 'user_12345'."

**🤖 AI Agent:**
> Here's the profile for user_12345: email is jane@example.com, signed up 3 months ago, last active 2 hours ago. Properties include plan:premium, company:Acme Inc, and role:admin. They've triggered 847 events including 120 pageviews and 45 purchases.


## ❓ FAQ

**Q: How do I create a PostHog Personal API Key?**
Log in to [**PostHog**](https://app.posthog.com), click your profile icon > **Personal API keys**, then **+ Create a Personal API Key**. Give it a label, select the required scopes and copy the key immediately — it won't be shown again after page refresh.

**Q: Can I toggle feature flags via the agent?**
Yes! Use `create_feature_flag` to add new flags, `update_feature_flag` to modify existing ones (name, description, enabled status), and `delete_feature_flag` to remove them. You'll need the numeric flag ID from `list_feature_flags` for update and delete operations.

**Q: What's the difference between events and persons?**
**Events** are actions that happen in your product (pageviews, button clicks, purchases). **Persons** are the users who perform those actions, identified by distinct_id. Events are linked to persons, so you can see what actions a specific user has taken. Use `list_events` to browse activity and `get_person` to see a user's profile.

**Q: Can I use this with a self-hosted PostHog instance?**
Yes! The tools default to `https://app.posthog.com` for the US cloud, but you can set the `host` parameter to your self-hosted instance URL (e.g. `https://posthog.yourcompany.com`). EU cloud users should set the host to `https://eu.posthog.com`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/posthog-alternative](https://vinkius.com/mcp/posthog-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PostHog** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `posthog-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PostHog** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "posthog-alternative": {
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
