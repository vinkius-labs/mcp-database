# SurveyMonkey Insights & Automation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/surveymonkey-insights-automation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

The automation side of SurveyMonkey: real-time response webhooks, contacts CRM with bulk import, organization/seat info, survey response trends and account checks — official API v3, OAuth long-lived token.

## Description
**SurveyMonkey automation and operations** as a single MCP server — the endpoints that make surveys event-driven, on the official API v3.

### What you can do
- **Account & org** — verify credentials via users/me; inspect your organization's teams and seats (enterprise)
- **Real-time webhooks** — create/list/delete subscriptions that PUSH every new response to your endpoint (responses_new, responses_updated, responses_completed, collector_new, survey_created) — build Slack alerts, live dashboards and CRM sync without polling
- **Contacts CRM** — list stored contacts; **bulk import** an entire audience (email, name, custom fields, list assignment) to seed email collector campaigns
- **Response trends** — time-bucketed completion data per survey for fatigue/seasonality analysis

### Authentication (from the official docs)
SurveyMonkey uses OAuth 2.0 authorization-code with **long-lived access tokens** (no refresh token): 1) send the user to `https://api.surveymonkey.com/oauth/authorize?response_type=code&client_id=...&redirect_uri=...&state=...`; 2) the returned code expires in 5 minutes; 3) exchange it at `POST https://api.surveymonkey.com/oauth/token` (form-encoded: client_id, client_secret, code, redirect_uri, grant_type=authorization_code). Paste the resulting token into this MCP's credentials. Rate limits: Private/Draft apps 120 req/min + 500 req/day; Public apps up to 500k/day; limits come back in `X-Ratelimit-App-Global-Day-*` headers.

### Pairs with the existing SurveyMonkey MCP
The published surveymonkey-mcp covers survey/page/question/collector/response CRUD. This one is the operations layer: webhooks, contacts, org and trends — zero tool overlap.

### Who is this for?
Ops teams automating survey pipelines, growth/CRM engineers, IT integrators and AI agents that need real-time survey signals.


## Available Tools (8)
- **get_organization**: Enterprise accounts only; returns 403 on personal plans.

Get your SurveyMonkey organization: teams, seats, users (enterprise view)
- **get_survey_trends**: Requires a paid plan with the trends feature; survey ids come from the published surveymonkey-mcp list_surveys.

Get response trends for a survey (time-bucketed completion data)
- **get_me_and_account**: The quickest credential sanity check and the source of account limits.

Get the authenticated user profile and account (users/me): username, plan, features
- **list_webhooks**: ) and status. Pair with create_webhook for event-driven survey pipelines.

List all configured webhooks (real-time push for responses and events)
- **create_webhook**: name: label; subscription_url: your HTTPS endpoint; object_type: "survey" (also collector/user); object_ids: survey ids to watch; event_type: "responses_new" (each new response), "responses_updated", "responses_completed", "collector_new" or "survey_created". SurveyMonkey POSTs the event JSON to your URL — real-time pipelines without polling.

Create a webhook: push survey responses to your endpoint in real time
- **delete_webhook**: Permanently removes the subscription — responses stop being pushed to the endpoint.

Delete a webhook by id (stop the real-time push)
- **list_contacts**: Paging via page/limit. Pair with bulk_import_contacts to seed thousands at once.

List stored contacts: emails, names, custom fields (survey recipient CRM)
- **bulk_import_contacts**: contacts: JSON array of {email, first_name?, last_name?, custom_field1..N?} (max ~100 per call); contact_list_id optionally adds them to a list. This is how you seed an email collector campaign with an entire audience programmatically.

Import contacts in bulk (CSV/JSON payloads) for email collector campaigns


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SurveyMonkey Insights & Automation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Alert our Slack every time someone completes the NPS survey"

**🤖 AI Agent:**
> 🔔 **Webhook created**

- Name: NPS responses → Slack
- Event: responses_completed (survey 12345678)
- Endpoint: https://hooks.yourco.com/sludge/nps
- Status: ✅ active

Every completed NPS response now POSTs to your middleware — pipe it into Slack. I can list or delete webhooks anytime.

---

**👤 You:**
> "Import these 50 conference attendees into our contacts for the follow-up campaign"

**🤖 AI Agent:**
> 📇 **Bulk import running**

50 contacts parsed (email + first name + company as custom_field1) and imported into contact list 'Conference 2026'.

Deduped against existing contacts. Ready to attach to an email collector — want me to verify by listing a sample?

---

**👤 You:**
> "Is my SurveyMonkey token still valid and what plan am I on?"

**🤖 AI Agent:**
> 🔍 **users/me check**

✅ Token valid — username: hr_ops@yourco.com
Plan: Advantage Annual
Features: custom variables ✓, email collectors ✓, trends ✓

Rate limits (Private app): 120 req/min, 500/day — X-Ratelimit headers show remaining counts on every call.


## ❓ FAQ

**Q: How do I get the access token?**
Register an app at developer.surveymonkey.com, then run the OAuth authorization-code flow: authorize URL (api.surveymonkey.com/oauth/authorize) → 5-minute code → exchange at POST api.surveymonkey.com/oauth/token (client_id, client_secret, code, redirect_uri, grant_type=authorization_code). The returned access token is long-lived — paste it into this MCP's credentials.

**Q: How is this different from the existing SurveyMonkey MCP?**
The published surveymonkey-mcp covers survey/page/question/collector/response CRUD. This MCP is the operations layer with zero overlap: webhooks (real-time push), contacts + bulk import, organization info, survey trends and users/me.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/surveymonkey-insights-automation](https://vinkius.com/ai-agent-connect/surveymonkey-insights-automation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SurveyMonkey Insights & Automation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surveymonkey-insights-automation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SurveyMonkey Insights & Automation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surveymonkey-insights-automation": {
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
